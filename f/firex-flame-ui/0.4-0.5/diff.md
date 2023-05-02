# Comparing `tmp/firex_flame_ui-0.4.tar.gz` & `tmp/firex_flame_ui-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydist/firex_flame_ui-0.4.tar", last modified: Thu May 30 11:02:57 2019, max compression
+gzip compressed data, was "dist/firex_flame_ui-0.5.tar", last modified: Mon Jun  3 15:57:05 2019, max compression
```

## Comparing `firex_flame_ui-0.4.tar` & `firex_flame_ui-0.5.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 djungic  (476191) eng         (25)        0 2019-05-30 11:02:57.000000 firex_flame_ui-0.4/
-drwxr-xr-x   0 djungic  (476191) eng         (25)        0 2019-05-30 11:02:57.000000 firex_flame_ui-0.4/dist/
-drwxr-xr-x   0 djungic  (476191) eng         (25)        0 2019-05-30 11:02:57.000000 firex_flame_ui-0.4/dist/css/
--rw-r--r--   0 djungic  (476191) eng         (25)     6947 2019-05-30 11:00:06.000000 firex_flame_ui-0.4/dist/css/app.e2e84099.css
--rw-r--r--   0 djungic  (476191) eng         (25)     1292 2019-05-30 11:00:07.000000 firex_flame_ui-0.4/dist/css/chunk-vendors.a2cbee8a.css
-drwxr-xr-x   0 djungic  (476191) eng         (25)        0 2019-05-30 11:02:57.000000 firex_flame_ui-0.4/dist/img/
--rw-r--r--   0 djungic  (476191) eng         (25)     7676 2019-05-30 11:00:07.000000 firex_flame_ui-0.4/dist/img/firex_logo.675380cb.png
-drwxr-xr-x   0 djungic  (476191) eng         (25)        0 2019-05-30 11:02:57.000000 firex_flame_ui-0.4/dist/js/
--rw-r--r--   0 djungic  (476191) eng         (25)    99352 2019-05-30 11:00:09.000000 firex_flame_ui-0.4/dist/js/app.19fe9253.js
--rw-r--r--   0 djungic  (476191) eng         (25)   559784 2019-05-30 11:00:11.000000 firex_flame_ui-0.4/dist/js/chunk-vendors.009e933e.js
--rw-r--r--   0 djungic  (476191) eng         (25)        0 2019-05-24 17:21:14.000000 firex_flame_ui-0.4/dist/__init__.py
--rw-r--r--   0 djungic  (476191) eng         (25)      742 2019-05-30 11:00:08.000000 firex_flame_ui-0.4/dist/index.html
-drwxr-xr-x   0 djungic  (476191) eng         (25)        0 2019-05-30 11:02:57.000000 firex_flame_ui-0.4/firex_flame_ui.egg-info/
--rw-r--r--   0 djungic  (476191) eng         (25)      254 2019-05-30 11:02:56.000000 firex_flame_ui-0.4/firex_flame_ui.egg-info/PKG-INFO
--rw-r--r--   0 djungic  (476191) eng         (25)      391 2019-05-30 11:02:56.000000 firex_flame_ui-0.4/firex_flame_ui.egg-info/SOURCES.txt
--rw-r--r--   0 djungic  (476191) eng         (25)        1 2019-05-30 11:02:55.000000 firex_flame_ui-0.4/firex_flame_ui.egg-info/dependency_links.txt
--rw-r--r--   0 djungic  (476191) eng         (25)       15 2019-05-30 11:02:55.000000 firex_flame_ui-0.4/firex_flame_ui.egg-info/top_level.txt
--rw-r--r--   0 djungic  (476191) eng         (25)        1 2019-05-24 17:03:32.000000 firex_flame_ui-0.4/firex_flame_ui.egg-info/zip-safe
--rw-r--r--   0 djungic  (476191) eng         (25)       83 2019-05-28 08:36:21.000000 firex_flame_ui-0.4/MANIFEST.in
--rw-r--r--   0 djungic  (476191) eng         (25)      713 2019-05-30 11:02:36.000000 firex_flame_ui-0.4/setup.py
--rw-r--r--   0 djungic  (476191) eng         (25)      254 2019-05-30 11:02:57.000000 firex_flame_ui-0.4/PKG-INFO
--rw-r--r--   0 djungic  (476191) eng         (25)       38 2019-05-30 11:02:57.000000 firex_flame_ui-0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/firex_flame_ui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/firex_flame_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/firex_flame_ui.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)      425 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/firex_flame_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      254 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/firex_flame_ui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       15 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/firex_flame_ui.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    68611 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/versioneer.py
+-rw-r--r--   0 root         (0) root         (0)      742 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/js/
+-rw-r--r--   0 root         (0) root         (0)   559784 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/js/chunk-vendors.88295e09.js
+-rw-r--r--   0 root         (0) root         (0)   102153 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/js/app.d2b5e0d8.js
+-rw-r--r--   0 root         (0) root         (0)      128 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1068 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/setup.py
+-rw-r--r--   0 root         (0) root         (0)       93 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      254 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18451 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/_version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       40 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/COMMITHASH
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/css/
+-rw-r--r--   0 root         (0) root         (0)     7038 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/css/app.2e01ad42.css
+-rw-r--r--   0 root         (0) root         (0)     1292 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/css/chunk-vendors.a2cbee8a.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-03 15:57:05.000000 firex_flame_ui-0.5/img/
+-rw-r--r--   0 root         (0) root         (0)     7676 2019-06-03 15:57:04.000000 firex_flame_ui-0.5/img/firex_logo.675380cb.png
```

### Comparing `firex_flame_ui-0.4/dist/css/app.e2e84099.css` & `firex_flame_ui-0.5/css/app.2e01ad42.css`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-.header[data-v-22bb7b42]{background-color:#eee;border-bottom:1px solid #000}@-webkit-keyframes spinner-data-v-22bb7b42{to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@keyframes spinner-data-v-22bb7b42{to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}.spinner[data-v-22bb7b42]:before{content:"";-webkit-box-sizing:border-box;box-sizing:border-box;position:absolute;top:50%;left:50%;width:20px;height:20px;margin-top:-10px;margin-left:-10px;border-radius:50%;border-top:2px solid #07d;border-right:2px solid transparent;-webkit-animation:spinner-data-v-22bb7b42 .6s linear infinite;animation:spinner-data-v-22bb7b42 .6s linear infinite}.notification[data-v-22bb7b42]{position:absolute;z-index:unset;display:inline-block;background:#00bfff;border-bottom:1px solid #000;width:100%;text-align:center;height:4em;line-height:4em}.flame-data[data-v-e080e642]{background:#fff;text-align:center;border:1px solid rgba(217,83,79,.8);color:#000;margin:3px;min-width:250px}a[data-v-e080e642]{color:inherit;cursor:pointer;text-decoration:none}.node[data-v-e080e642]{font-family:Source Sans Pro,sans-serif;font-weight:400;font-style:normal;color:#fff;padding:3px;display:block;border-right:1px solid #fff;border-bottom:1px solid #fff}.node[data-v-e080e642]:hover{background:#000!important}.flame-data a[data-v-e080e642]{display:inline-block}.retries[data-v-e080e642]{position:absolute;right:6px;font-size:11px;top:2px}.retries-img[data-v-e080e642]{position:absolute;right:1px;height:16px}.stacked-effect[data-v-4256192c]{border:.5px solid #fff;border-radius:8px;position:absolute;top:0}.stacks-link:hover .stacked-effect[data-v-4256192c]{cursor:pointer;background:#000!important}.stacks-link[data-v-4256192c]{position:absolute;top:0;z-index:-1;display:inline-block}.stacks-link:hover .stacks-count[data-v-4256192c]{cursor:pointer}.stacks-count[data-v-4256192c]{position:absolute;bottom:1px;text-align:center;width:100%;color:#fff;font-size:13px;font-family:Source Sans Pro,sans-serif;height:1em}.faded[data-v-4af60d56]{opacity:.3}.fade-enter-active[data-v-4af60d56]{-webkit-transition:opacity 2s;transition:opacity 2s}.fade-enter[data-v-4af60d56]{opacity:.1}.link[data-v-719e8d6a]{fill:none;stroke:#000;stroke-width:2px}[data-v-7e9020b6]{-webkit-box-sizing:border-box;box-sizing:border-box}#chart-container[data-v-7e9020b6]{background:#fff;display:-webkit-box;display:-ms-flexbox;display:flex;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;justify-content:center;height:100%;width:100%}.header[data-v-061bf61e]{background-color:#eee;border-bottom:1px solid #000}.uid[data-v-061bf61e]{margin:0 8px;padding:0;white-space:nowrap;font-weight:400}.flame-link[data-v-061bf61e],.uid[data-v-061bf61e]{font-family:Source Sans Pro,sans-serif;font-size:20px;line-height:40px}.flame-link[data-v-061bf61e]{vertical-align:top;border-left:1px solid #000;text-align:center;text-decoration:none;padding:0 8px;color:#000;border-radius:0;-webkit-box-pack:end;-ms-flex-pack:end;justify-content:flex-end}.flame-link a[data-v-061bf61e]{text-decoration:none}.header-icon-button[data-v-061bf61e]{padding:0 4px;border-left:1px solid #000;-webkit-box-pack:end;-ms-flex-pack:end;justify-content:end;font-size:20px;line-height:40px;cursor:pointer;color:#000}.header-icon-button[data-v-061bf61e]:hover{color:#2980ff}a[data-v-061bf61e]{color:#000}a[data-v-061bf61e]:hover{color:#2980ff}.kill-button[data-v-061bf61e]{color:#900}.kill-button[data-v-061bf61e]:hover{color:#fff;background:#900}.header-popover[data-v-061bf61e]{padding:3px;font-size:13px;line-height:1em;border-color:#000;border-radius:0;-webkit-box-shadow:2px 1px 1px #3a3a3a;box-shadow:2px 1px 1px #3a3a3a}.collapse-menu[data-v-0de53894]{text-align:left;font-family:Source Sans Pro,sans-serif;cursor:auto;font-size:20px}.collapse-button[data-v-0de53894]{font-size:20px;line-height:40px;cursor:pointer;color:#000}.collapse-button[data-v-0de53894]:hover,.collapse-menu-item[data-v-0de53894]:hover{color:#2980ff;cursor:pointer}.search[data-v-409babf4]{line-height:36px;border:2px solid #2980b9;outline:0;font-size:24px;vertical-align:top;width:300px;padding:0 2px}.search-pos[data-v-409babf4],.search[data-v-409babf4]{font-family:Source Sans Pro,sans-serif;display:inline-block}.search-pos[data-v-409babf4]{color:#000;line-height:40px;font-size:20px;cursor:default}.list-container[data-v-2470f47c]{-webkit-box-flex:1;-ms-flex:1;flex:1;overflow:auto;-webkit-box-align:center;-ms-flex-align:center;align-items:center;display:-webkit-box;display:-ms-flexbox;display:flex;-webkit-box-orient:vertical;-webkit-box-direction:normal;-ms-flex-direction:column;flex-direction:column}.time-table[data-v-65363fc0]{font-family:Source Sans Pro,sans-serif}table[data-v-65363fc0]{border:none}td[data-v-65363fc0]{width:auto}td.min[data-v-65363fc0]{width:1%;white-space:nowrap}tr[data-v-65363fc0]:hover{background-color:#add8e6}.sortable-header[data-v-65363fc0]{white-space:nowrap}.sortable-header[data-v-65363fc0]:hover{cursor:pointer;color:#2980ff}.task[data-v-65363fc0]:hover{background:#000!important}.popover-container[data-v-65363fc0]{background:#fff;padding:0;text-align:left;border:1px solid #000;font-family:Source Sans Pro,sans-serif}.popover-title[data-v-65363fc0]{padding:3px;text-align:center;border-bottom:1px solid #000;background-color:#eee}.icon-links a[data-v-65363fc0]{padding:3px;color:#000}.icon-links a[data-v-65363fc0]:hover{color:#2980ff}.node-attributes[data-v-39c046bc]{font-family:Source Code Pro,monospace;font-size:14px;margin:10px;-webkit-box-flex:1;-ms-flex:1;flex:1;overflow:auto;display:-webkit-box;display:-ms-flexbox;display:flex;-webkit-box-orient:vertical;-webkit-box-direction:normal;-ms-flex-direction:column;flex-direction:column}h1[data-v-6453f82e]{font-size:1.4em;margin-bottom:0;font-weight:700}ul li[data-v-6453f82e]{padding:12px;max-width:540px;text-align:center;display:inline-table;border-left:1px solid #000}ul li[data-v-6453f82e]:first-child{border:0}.help-content[data-v-6453f82e]{font-family:Source Sans Pro,sans-serif;margin:10px}.node-type[data-v-6453f82e]{text-align:center;font-weight:400}.settings{font-family:Source Sans Pro,sans-serif;margin:10px}.display-config td{border:1px solid #cbcbcb;border-spacing:0;padding:5px}.display-config{border-spacing:0}.display-config thead{font-weight:700}h1[data-v-173d11f4]{font-family:Source Sans Pro,sans-serif;font-size:1.4em;margin-bottom:0}.help-content[data-v-173d11f4]{font-family:Source Sans Pro,sans-serif;margin:10px;font-size:1em}.shortcuts[data-v-173d11f4]{font-size:1.2em;-webkit-column-count:2;column-count:2}ul[data-v-173d11f4]{text-align:center;padding-left:0;margin:0;list-style:none}.shortcuts li[data-v-173d11f4]{width:100%;border:0;display:inline-block;text-align:left}ul li[data-v-173d11f4]{padding:12px;max-width:540px;text-align:center;display:inline-table;border-left:1px solid #000}body{margin:0}body,html{margin:0}#app,body,html{height:100%}
+.header[data-v-22bb7b42]{background-color:#eee;border-bottom:1px solid #000}@-webkit-keyframes spinner-data-v-22bb7b42{to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@keyframes spinner-data-v-22bb7b42{to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}.spinner[data-v-22bb7b42]:before{content:"";-webkit-box-sizing:border-box;box-sizing:border-box;position:absolute;top:50%;left:50%;width:20px;height:20px;margin-top:-10px;margin-left:-10px;border-radius:50%;border-top:2px solid #07d;border-right:2px solid transparent;-webkit-animation:spinner-data-v-22bb7b42 .6s linear infinite;animation:spinner-data-v-22bb7b42 .6s linear infinite}.notification[data-v-22bb7b42]{position:absolute;z-index:unset;display:inline-block;background:#00bfff;border-bottom:1px solid #000;width:100%;text-align:center;height:4em;line-height:4em}.flame-data[data-v-19c0b619]{background:#fff;text-align:center;border:1px solid rgba(217,83,79,.8);color:#000;margin:3px;min-width:250px}a[data-v-19c0b619]{color:inherit;cursor:pointer;text-decoration:none}.node[data-v-19c0b619]{font-family:Source Sans Pro,sans-serif;font-weight:400;font-style:normal;color:#fff;padding:3px;display:block;border-right:1px solid #fff;border-bottom:1px solid #fff}.node[data-v-19c0b619]:hover{background:#000!important}.flame-data a[data-v-19c0b619]{display:inline-block}.retries[data-v-19c0b619]{position:absolute;right:6px;font-size:11px;top:2px}.retries-img[data-v-19c0b619]{position:absolute;right:1px;height:16px}.stacked-effect[data-v-4256192c]{border:.5px solid #fff;border-radius:8px;position:absolute;top:0}.stacks-link:hover .stacked-effect[data-v-4256192c]{cursor:pointer;background:#000!important}.stacks-link[data-v-4256192c]{position:absolute;top:0;z-index:-1;display:inline-block}.stacks-link:hover .stacks-count[data-v-4256192c]{cursor:pointer}.stacks-count[data-v-4256192c]{position:absolute;bottom:1px;text-align:center;width:100%;color:#fff;font-size:13px;font-family:Source Sans Pro,sans-serif;height:1em}.faded[data-v-4af60d56]{opacity:.3}.fade-enter-active[data-v-4af60d56]{-webkit-transition:opacity 2s;transition:opacity 2s}.fade-enter[data-v-4af60d56]{opacity:.1}.link[data-v-719e8d6a]{fill:none;stroke:#000;stroke-width:2px}[data-v-7e9020b6]{-webkit-box-sizing:border-box;box-sizing:border-box}#chart-container[data-v-7e9020b6]{background:#fff;display:-webkit-box;display:-ms-flexbox;display:flex;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;justify-content:center;height:100%;width:100%}.flame-link{vertical-align:top;border-left:1px solid #000;line-height:40px;text-align:center;padding:0 8px;color:#000;border-radius:0;font-size:20px;-webkit-box-pack:end;-ms-flex-pack:end;justify-content:flex-end}.flame-link,.flame-link a{font-family:Source Sans Pro,sans-serif;text-decoration:none}.header-icon-button{-webkit-box-pack:end;-ms-flex-pack:end;justify-content:end;cursor:pointer}.header-icon-button:hover{color:#2980ff}a{color:#000}a:hover{color:#2980ff}.header-popover{padding:3px;font-size:13px;line-height:1em;border-color:#000;border-radius:0;-webkit-box-shadow:2px 1px 1px #3a3a3a;box-shadow:2px 1px 1px #3a3a3a}.header[data-v-5a00c5be]{background-color:#eee;border-bottom:1px solid #000}.uid[data-v-5a00c5be]{font-family:Source Sans Pro,sans-serif;margin:0 8px;padding:0;white-space:nowrap;font-size:20px;line-height:40px;font-weight:400}a[data-v-5a00c5be]{color:#000}a[data-v-5a00c5be]:hover{color:#2980ff}.kill-button[data-v-5a00c5be]{color:#900}.kill-button[data-v-5a00c5be]:hover{color:#fff;background:#900}.collapse-menu[data-v-ac58f39e]{text-align:left;font-family:Source Sans Pro,sans-serif;cursor:auto;font-size:20px}.collapse-button[data-v-ac58f39e]{font-size:20px;line-height:40px;cursor:pointer;color:#000}.collapse-button[data-v-ac58f39e]:hover,.collapse-menu-item[data-v-ac58f39e]:hover{color:#2980ff;cursor:pointer}[data-v-ac58f39e] .flame-link{padding-right:0}.search[data-v-6ee28668]{line-height:36px;border:2px solid #2980b9;outline:0;font-size:24px;vertical-align:top;width:300px;padding:0 2px}.search-pos[data-v-6ee28668],.search[data-v-6ee28668]{font-family:Source Sans Pro,sans-serif;display:inline-block}.search-pos[data-v-6ee28668]{color:#000;line-height:40px;font-size:20px;cursor:default;padding:0 5px}[data-v-6ee28668] .flame-link{border:none}.list-container[data-v-d2e6a2bc]{-webkit-box-flex:1;-ms-flex:1;flex:1;overflow:auto;-webkit-box-align:center;-ms-flex-align:center;align-items:center;display:-webkit-box;display:-ms-flexbox;display:flex;-webkit-box-orient:vertical;-webkit-box-direction:normal;-ms-flex-direction:column;flex-direction:column}.time-table[data-v-53a20b2c]{font-family:Source Sans Pro,sans-serif}table[data-v-53a20b2c]{border:none}td[data-v-53a20b2c]{width:auto}td.min[data-v-53a20b2c]{width:1%;white-space:nowrap}tr[data-v-53a20b2c]:hover{background-color:#add8e6}.sortable-header[data-v-53a20b2c]{white-space:nowrap}.sortable-header[data-v-53a20b2c]:hover{cursor:pointer;color:#2980ff}.task[data-v-53a20b2c]:hover{background:#000!important}.popover-container[data-v-53a20b2c]{background:#fff;padding:0;text-align:left;border:1px solid #000;font-family:Source Sans Pro,sans-serif}.popover-title[data-v-53a20b2c]{padding:3px;text-align:center;border-bottom:1px solid #000;background-color:#eee}.icon-links a[data-v-53a20b2c]{padding:3px;color:#000}.icon-links a[data-v-53a20b2c]:hover{color:#2980ff}.state-rect[data-v-53a20b2c]:hover{-webkit-box-shadow:0 3px 3px #3a3a3a;box-shadow:0 3px 3px #3a3a3a;z-index:10}.node-attributes[data-v-192505f8]{font-family:Source Code Pro,monospace;font-size:14px;margin:10px;-webkit-box-flex:1;-ms-flex:1;flex:1;overflow:auto;display:-webkit-box;display:-ms-flexbox;display:flex;-webkit-box-orient:vertical;-webkit-box-direction:normal;-ms-flex-direction:column;flex-direction:column}h1[data-v-6453f82e]{font-size:1.4em;margin-bottom:0;font-weight:700}ul li[data-v-6453f82e]{padding:12px;max-width:540px;text-align:center;display:inline-table;border-left:1px solid #000}ul li[data-v-6453f82e]:first-child{border:0}.help-content[data-v-6453f82e]{font-family:Source Sans Pro,sans-serif;margin:10px}.node-type[data-v-6453f82e]{text-align:center;font-weight:400}.settings{font-family:Source Sans Pro,sans-serif;margin:10px}.display-config td{border:1px solid #cbcbcb;border-spacing:0;padding:5px}.display-config{border-spacing:0}.display-config thead{font-weight:700}h1[data-v-173d11f4]{font-family:Source Sans Pro,sans-serif;font-size:1.4em;margin-bottom:0}.help-content[data-v-173d11f4]{font-family:Source Sans Pro,sans-serif;margin:10px;font-size:1em}.shortcuts[data-v-173d11f4]{font-size:1.2em;-webkit-column-count:2;column-count:2}ul[data-v-173d11f4]{text-align:center;padding-left:0;margin:0;list-style:none}.shortcuts li[data-v-173d11f4]{width:100%;border:0;display:inline-block;text-align:left}ul li[data-v-173d11f4]{padding:12px;max-width:540px;text-align:center;display:inline-table;border-left:1px solid #000}body{margin:0}body,html{margin:0}#app,body,html{height:100%}
```

### Comparing `firex_flame_ui-0.4/dist/css/chunk-vendors.a2cbee8a.css` & `firex_flame_ui-0.5/css/chunk-vendors.a2cbee8a.css`

 * *Files identical despite different names*

### Comparing `firex_flame_ui-0.4/dist/img/firex_logo.675380cb.png` & `firex_flame_ui-0.5/img/firex_logo.675380cb.png`

 * *Files identical despite different names*

### Comparing `firex_flame_ui-0.4/dist/js/app.19fe9253.js` & `firex_flame_ui-0.5/js/app.d2b5e0d8.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -71,63 +71,59 @@
     for (var l = 0; l < o.length; l++) e(o[l]);
     var c = u;
     n.push([0, "chunk-vendors"]), a()
 })({
     0: function(t, e, a) {
         t.exports = a("56d7")
     },
+    "02d7": function(t, e, a) {},
     "034f": function(t, e, a) {
         "use strict";
         var i = a("64a9"),
             s = a.n(i);
         s.a
     },
     "05c2": function(t, e, a) {},
     "0ef1": function(t, e, a) {},
     1: function(t, e) {},
-    "16c8": function(t, e, a) {
+    1723: function(t, e, a) {
         "use strict";
-        var i = a("7f21"),
+        var i = a("e229"),
             s = a.n(i);
         s.a
     },
-    1723: function(t, e, a) {
+    "177d": function(t, e, a) {
         "use strict";
-        var i = a("e229"),
+        var i = a("4ea5"),
             s = a.n(i);
         s.a
     },
-    "26ad": function(t, e, a) {
+    2638: function(t, e, a) {
         "use strict";
-        var i = a("c3ca"),
+        var i = a("d32c"),
             s = a.n(i);
         s.a
     },
     "27c0": function(t, e, a) {
         t.exports = a.p + "img/firex_logo.675380cb.png"
     },
-    "38ca": function(t, e, a) {},
+    "34b2": function(t, e, a) {},
     "4d1a": function(t, e, a) {
         "use strict";
         var i = a("6604"),
             s = a.n(i);
         s.a
     },
     "4e67": function(t, e, a) {
         "use strict";
         var i = a("cfad"),
             s = a.n(i);
         s.a
     },
-    "52f7": function(t, e, a) {
-        "use strict";
-        var i = a("38ca"),
-            s = a.n(i);
-        s.a
-    },
+    "4ea5": function(t, e, a) {},
     "56d7": function(t, e, a) {
         "use strict";
         a.r(e);
         a("cadf"), a("551c"), a("f751"), a("097d");
         var i = a("2b0e"),
             s = a("3003"),
             n = a("ecee"),
@@ -190,20 +186,20 @@
             },
             E = [],
             O = a("15b8"),
             R = a.n(O),
             I = (a("4917"), a("2ef0")),
             $ = a.n(I),
             L = (a("7f7f"), a("795b")),
-            P = a.n(L),
-            F = a("8055"),
-            M = a.n(F);
+            F = a.n(L),
+            P = a("8055"),
+            M = a.n(P);
 
         function Q(t, e, a, i, s) {
-            var n = new P.a(function(n, r) {
+            var n = new F.a(function(n, r) {
                 var o = !1;
                 t.on(a, function(t) {
                     o = !0, n(t)
                 }), $.a.isNil(i) || t.on(i, function(t) {
                     o = !0, r(t)
                 }), $.a.isNil(s) || setTimeout(function() {
                     o || r({
@@ -272,19 +268,19 @@
             return q.getTaskGraph()
         }
 
         function z(t) {
             return q.fetchTaskDetails(t)
         }
 
-        function G(t) {
+        function V(t) {
             return q.fetchTaskFields(t)
         }
 
-        function V(t) {
+        function G(t) {
             return q.startLiveUpdate(t)
         }
 
         function Y() {
             return q.stopLiveUpdate()
         }
 
@@ -484,51 +480,56 @@
                 return (t ^ crypto.getRandomValues(new Uint8Array(1))[0] & 15 >> t / 4).toString(16)
             })
         }
         var kt = "#2A2",
             vt = {
                 "task-received": {
                     background: "#888",
-                    priority: 6
+                    priority: 6,
+                    display: "Received"
                 },
                 "task-blocked": {
                     background: "#888",
-                    priority: 7
+                    priority: 7,
+                    display: "Blocked"
                 },
                 "task-started": {
                     background: "cornflowerblue",
-                    priority: 1
+                    priority: 1,
+                    display: "In-Progress"
                 },
                 "task-succeeded": {
                     background: kt,
-                    priority: 9
+                    priority: 9,
+                    display: "Success"
                 },
                 "task-shutdown": {
                     background: kt,
-                    priority: 10
+                    priority: 10,
+                    display: "Success"
                 },
                 "task-failed": {
                     background: "#900",
-                    priority: 3
+                    priority: 3,
+                    display: "Failed"
                 },
                 "task-revoked": {
                     background: "#F40",
-                    priority: 4
+                    priority: 4,
+                    display: "Revoked"
                 },
                 "task-incomplete": {
                     background: "repeating-linear-gradient(45deg,#888,#888 5px,#444 5px,#444 10px)",
-                    priority: 5
-                },
-                "task-completed": {
-                    background: "#AAA",
-                    priority: 8
+                    priority: 5,
+                    display: "Incomplete"
                 },
                 "task-unblocked": {
                     background: "cornflowerblue",
-                    priority: 2
+                    priority: 2,
+                    display: "In-Progress"
                 }
             };
 
         function At(t, e) {
             if (rt(t)) return "repeating-linear-gradient(45deg,#888,#888 5px,#893C3C 5px,#F71818  10px)";
             var a = "#888";
             return $.a.get(vt, [e, "background"], a)
@@ -537,21 +538,27 @@
         function Ct(t) {
             var e = $.a.minBy(t, function(t) {
                 return $.a.get(vt, [t, "priority"], 1e3)
             });
             return At(null, e)
         }
 
-        function Ut(t, e, a) {
-            return xt(t, e, null, a)
+        function Ut(t) {
+            return $.a.get(vt, t, {
+                display: "Unknown"
+            }).display
+        }
+
+        function xt(t, e, a) {
+            return St(t, e, null, a)
         }
 
-        function xt(t, e, a, i) {
+        function St(t, e, a, i) {
             var s = $.a.map(e[t], function(a) {
-                    return xt(a, e, t, i)
+                    return St(a, e, t, i)
                 }),
                 n = $.a.reduce(s, $.a.merge, {}),
                 r = $.a.filter(e[t], function(t) {
                     return i[t]
                 }),
                 o = $.a.flatMap(r, function(t) {
                     return [t].concat(n[t].collapsedUuids)
@@ -565,69 +572,69 @@
                 })
             }), $.a.assign(Object(tt["a"])({}, [t], {
                 collapsedUuids: o,
                 parentId: a
             }), n)
         }
 
-        function St(t, e, a, i) {
+        function _t(t, e, a, i) {
             var s = -(new Date).getTime();
             return $.a.mapValues($.a.keyBy(t), function() {
                 return {
                     targets: [a],
                     operation: e,
                     priority: s,
                     stateSource: "ui",
                     sourceTaskUuid: i
                 }
             })
         }
 
-        function _t() {
+        function Bt() {
             if ($.a.has(localStorage, "displayConfigs")) try {
                 return JSON.parse(localStorage.getItem("displayConfigs"))
             } catch (t) {
                 localStorage.removeItem("displayConfigs")
             }
             return []
         }
 
-        function Bt(t, e) {
+        function Dt(t, e) {
             if ($.a.isArray(t)) return t.concat(e)
         }
 
-        function Dt(t, e) {
+        function bt(t, e) {
             return 0 === $.a.difference(e, t).length
         }
 
-        function bt(t, e) {
+        function Tt(t, e) {
             return $.a.some(t, function(t) {
                 return $.a.includes(e, t)
             })
         }
 
-        function Tt(t) {
+        function wt(t) {
             var e = Boolean(t);
             return e ? "" : "8px"
         }
 
-        function wt(t, e) {
+        function Nt(t, e) {
             var a = $.a.pickBy(e, function(e, a) {
                     return !$.a.has(t, a)
                 }),
                 i = $.a.pickBy(e, function(e, a) {
                     return $.a.has(t, a)
                 }),
                 s = W()({}, t, a);
             return $.a.each(i, function(e, a) {
                 s[a] = W()({}, t[a], e)
             }), s
         }
-        var Nt = new i["a"],
-            Et = {
+        var Et = new i["a"],
+            Ot = {
                 name: "XTasksParent",
                 props: {
                     inputLogDir: {
                         required: !1,
                         type: String
                     },
                     inputFlameServer: {
@@ -678,19 +685,19 @@
                     },
                     isApiConnected: function() {
                         return this.$store.state.tasks.apiConnected
                     }
                 },
                 created: function() {
                     var t = this;
-                    Nt.$on("revoke-root", function() {
+                    Et.$on("revoke-root", function() {
                         t.revokeTask(t.rootUuid)
-                    }), Nt.$on("revoke-task", function(e) {
+                    }), Et.$on("revoke-task", function(e) {
                         t.revokeTask(e)
-                    }), Nt.$on("graph-refresh", function() {
+                    }), Et.$on("graph-refresh", function() {
                         t.updateFullTasksState(t.liveUpdate)
                     })
                 },
                 methods: {
                     fetchNodesByUuidFromRecFile: function(t) {
                         return fetch(t).then(function(t) {
                             return t.text()
@@ -705,18 +712,18 @@
                         this.$store.dispatch("tasks/addTasksData", this.newTaskDataToDispatch), this.newTaskDataToDispatch = {}
                     }, 500, {
                         maxWait: 1500,
                         leading: !0,
                         trailing: !0
                     }),
                     mergeNodesByUuid: function(t) {
-                        this.newTaskDataToDispatch = R()(wt(this.newTaskDataToDispatch, t)), this.debouncedDispatchTasksUpdate()
+                        this.newTaskDataToDispatch = R()(Nt(this.newTaskDataToDispatch, t)), this.debouncedDispatchTasksUpdate()
                     },
                     startLiveUpdate: function() {
-                        V(this.mergeNodesByUuid)
+                        G(this.mergeNodesByUuid)
                     },
                     updateFullTasksState: function(t) {
                         var e = this;
                         this.updating = !0;
                         var a = K();
                         t && a.then(function(t) {
                             return e.startLiveUpdate(), t
@@ -791,19 +798,19 @@
                                     return e.$store.commit("tasks/setApiConnected", !1)
                                 }
                             }), this.fetchAllTasksAndStartLiveUpdate(), this.setFlameRunMetadata()
                         }
                     }
                 }
             },
-            Ot = Et,
-            Rt = (a("9048"), a("2877")),
-            It = Object(Rt["a"])(Ot, N, E, !1, null, "22bb7b42", null),
-            $t = It.exports,
-            Lt = function() {
+            Rt = Ot,
+            It = (a("9048"), a("2877")),
+            $t = Object(It["a"])(Rt, N, E, !1, null, "22bb7b42", null),
+            Lt = $t.exports,
+            Ft = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticStyle: {
                         width: "100%",
                         height: "100%",
@@ -833,26 +840,25 @@
                         links: t.headerParams.links,
                         legacyPath: t.headerParams.legacyPath
                     },
                     scopedSlots: t._u([{
                         key: "prebuttons",
                         fn: function() {
                             return [a("x-task-node-search", {
-                                staticClass: "header-icon-button",
                                 attrs: {
                                     findUncollapsedAncestor: !0
                                 }
                             }), a("x-collapse-buttons")]
                         },
                         proxy: !0
                     }])
                 }), t.runMetadata.uid ? a("x-graph") : t._e()], 1)
             },
             Pt = [],
-            Ft = function() {
+            Mt = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticStyle: {
                         width: "100%",
                         height: "100%",
@@ -898,20 +904,20 @@
                     }
                 }), a("x-svg-task-nodes", {
                     attrs: {
                         nodeLayoutsByUuid: t.nodeLayoutsByUuid
                     }
                 })], 1)])]), a("x-task-capturing-nodes")], 1)
             },
-            Mt = [],
-            Qt = a("cebc"),
-            Xt = a("d934"),
-            qt = a("fd32"),
-            jt = a("2f62"),
-            Ht = function() {
+            Qt = [],
+            Xt = a("cebc"),
+            qt = a("d934"),
+            jt = a("fd32"),
+            Ht = a("2f62"),
+            Kt = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("transition-group", {
                     attrs: {
                         name: t.fadeTransitionName,
                         tag: "g"
@@ -937,16 +943,16 @@
                             taskUuid: i,
                             width: e.width,
                             height: e.height
                         }
                     })], 1)], 1)
                 }), 0)
             },
-            Kt = [],
-            zt = function() {
+            zt = [],
+            Vt = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     style: {
                         "margin-left": t.allStackOffset + "px",
                         display: "inline-block"
@@ -975,15 +981,15 @@
                 }), a("div", {
                     staticClass: "stacks-count"
                 }, [t._v("\n      " + t._s(t.collapsedUuidsCount) + " " + t._s(1 === t.collapsedUuidsCount ? "Task" : "Tasks") + "\n    ")])], 2) : t._e()])
             },
             Gt = [];
         a("3b2b");
 
-        function Vt(t, e) {
+        function Yt(t, e) {
             var a = {
                     flameData: 5,
                     userConfig: 4,
                     runState: 3
                 },
                 i = $.a.get(a, e, 6);
             return $.a.mapValues(t, function(t) {
@@ -992,15 +998,15 @@
                         priority: i,
                         stateSource: e
                     }, t)
                 })
             })
         }
 
-        function Yt(t, e) {
+        function Jt(t, e) {
             var a = $.a.flatMap(t, function(t) {
                 var a, i;
                 if ($.a.has(t, ["source_node", "value"])) {
                     var s = ht(t.source_node.value, e);
                     s.push(t.source_node.value), i = $.a.pick(e, s)
                 } else i = e;
                 if ("task_name" === t.relative_to_nodes.type) {
@@ -1024,15 +1030,15 @@
             return $.a.mapValues($.a.groupBy(a, "task_uuid"), function(t) {
                 return $.a.map(t, function(t) {
                     return $.a.pick(t, ["operation", "targets"])
                 })
             })
         }
 
-        function Jt(t, e, a, i) {
+        function Zt(t, e, a, i) {
             var s;
             if (e) {
                 var n = $.a.some($.a.get(i, t, []), function(t) {
                     return "collapse" === t.operation && $.a.isEqual(t.targets, ["descendants"])
                 });
                 s = n ? {
                     uuids: [t],
@@ -1071,15 +1077,15 @@
                 uuids: [t],
                 operation: "collapse",
                 target: "descendants"
             };
             return s
         }
 
-        function Zt(t, e, a) {
+        function Wt(t, e, a) {
             var i = $.a.keyBy($.a.map(t, function(t, e) {
                     return {
                         uuid: t,
                         distance: e + 1
                     }
                 }), "uuid"),
                 s = $.a.mapValues(e, function(t) {
@@ -1093,22 +1099,22 @@
                             distance: i[e].distance
                         }, t)
                     })
                 });
             return $.a.flatten($.a.values(n))
         }
 
-        function Wt(t, e, a, i) {
+        function te(t, e, a, i) {
             var s = {
                     self: $.a.filter($.a.get(e, t, []), function(t) {
                         return $.a.includes(t.targets, "self")
                     }),
-                    ancestor: Zt(a, $.a.pick(e, a), "descendants"),
-                    descendant: Zt(i, $.a.pick(e, i), "ancestors"),
-                    grandparent: Zt($.a.tail(a), $.a.pick(e, $.a.tail(a)), "grandchildren")
+                    ancestor: Wt(a, $.a.pick(e, a), "descendants"),
+                    descendant: Wt(i, $.a.pick(e, i), "ancestors"),
+                    grandparent: Wt($.a.tail(a), $.a.pick(e, $.a.tail(a)), "grandchildren")
                 },
                 n = {
                     self: 1,
                     ancestor: 2,
                     descendant: 3,
                     grandparent: 4
                 },
@@ -1123,36 +1129,36 @@
                         targetPriority: n[e],
                         opPriority: r[t.operation]
                     }, $.a.omit(t, ["targets"]))
                 })
             })
         }
 
-        function te(t, e, a, i) {
-            var s = Wt(t, e, a, i),
+        function ee(t, e, a, i) {
+            var s = te(t, e, a, i),
                 n = $.a.sortBy(s, ["priority", "opPriority", "targetPriority", "distance"]);
             return $.a.head(n)
         }
 
-        function ee(t, e, a) {
+        function ae(t, e, a) {
             var i = {},
                 s = [t];
             while (s.length > 0) {
                 var n = s.pop(),
-                    r = te(n, a, e[n].ancestorUuids, e[n].descendantUuids);
+                    r = ee(n, a, e[n].ancestorUuids, e[n].descendantUuids);
                 i[n] = {
                     collapsed: !$.a.isUndefined(r) && "collapse" === r.operation,
                     minPriorityOp: r
                 }, s = s.concat(e[n].childrenUuids)
             }
             return i[t].collapsed = !1, i
         }
-        var ae = 12,
-            ie = 2,
-            se = function() {
+        var ie = 12,
+            se = 2,
+            ne = function() {
                 var t = this,
                     e = t.$createElement,
                     i = t._self._c || e;
                 return i("router-link", {
                     attrs: {
                         to: t.allowClickToAttributes ? t.routeToAttribute() : t.currentRoute()
                     }
@@ -1260,25 +1266,25 @@
                     attrs: {
                         runState: t.runState,
                         firstStarted: t.firstStarted,
                         actualRuntime: t.actualRuntime
                     }
                 })], 1)])])])
             },
-            ne = [],
-            re = function() {
+            re = [],
+            oe = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", [t._v(t._s(t.duration))])
             },
-            oe = [],
-            ue = a("0a0d"),
-            le = a.n(ue),
-            ce = {
+            ue = [],
+            le = a("0a0d"),
+            ce = a.n(le),
+            de = {
                 name: "XDuration",
                 props: {
                     runState: {
                         required: !0
                     },
                     firstStarted: {
                         required: !0
@@ -1291,15 +1297,15 @@
                     return {
                         liveRunTime: 0
                     }
                 },
                 created: function() {
                     this.updateLiveRuntimeAndSchedule()
                 },
-                computed: Object(Qt["a"])({}, Object(jt["c"])({
+                computed: Object(Xt["a"])({}, Object(Ht["c"])({
                     liveUpdate: function(t) {
                         return t.graph.liveUpdate
                     }
                 }), {
                     duration: function() {
                         var t;
                         if (!pt(this.runState) && this.actualRuntime) t = this.actualRuntime;
@@ -1309,27 +1315,27 @@
                         }
                         return "time: ".concat(gt(t))
                     }
                 }),
                 methods: {
                     updateLiveRuntimeAndSchedule: function() {
                         var t = this;
-                        this.liveUpdate && pt(this.runState) && this.firstStarted && (this.liveRunTime = le()() / 1e3 - this.firstStarted, setTimeout(function() {
+                        this.liveUpdate && pt(this.runState) && this.firstStarted && (this.liveRunTime = ce()() / 1e3 - this.firstStarted, setTimeout(function() {
                             t.liveUpdate && t.updateLiveRuntimeAndSchedule()
                         }, 3e3))
                     }
                 }
             },
-            de = ce,
-            pe = Object(Rt["a"])(de, re, oe, !1, null, "34a6e136", null),
-            fe = pe.exports,
-            he = {
+            pe = de,
+            fe = Object(It["a"])(pe, oe, ue, !1, null, "34a6e136", null),
+            he = fe.exports,
+            ge = {
                 name: "XNode",
                 components: {
-                    XDuration: fe
+                    XDuration: he
                 },
                 props: {
                     allowCollapse: {
                         default: !0
                     },
                     taskUuid: {
                         required: !0
@@ -1402,15 +1408,15 @@
                     },
                     minPriorityOp: function() {
                         return this.$store.getters["graph/resolvedCollapseStateByUuid"][this.taskUuid].minPriorityOp
                     },
                     topLevelStyle: function() {
                         var t = {
                             background: At(this.exception, this.runState),
-                            "border-radius": Tt(this.chainDepth)
+                            "border-radius": wt(this.chainDepth)
                         };
                         return this.fromPlugin && (t.border = "2px dashed #000"), t
                     },
                     showLegacyFlameAdditionalData: function() {
                         return !$.a.includes($.a.map($.a.get(this.task, "flame_data", {}), "type"), "html")
                     },
                     flameDataHtmlContent: function() {
@@ -1423,15 +1429,15 @@
                     this.emit_dimensions()
                 },
                 updated: function() {
                     this.emit_dimensions()
                 },
                 methods: {
                     emitCollapseToggle: function() {
-                        Nt.$emit("toggle-task-collapse", this.taskUuid)
+                        Et.$emit("toggle-task-collapse", this.taskUuid)
                     },
                     routeToAttribute: function() {
                         return ct(this.$route.query, "XNodeAttributes", {
                             uuid: this.taskUuid
                         })
                     },
                     currentRoute: function() {
@@ -1458,36 +1464,36 @@
                                 };
                                 $.a.isEqual(t.latestEmittedDimensions, s) || (t.latestEmittedDimensions = s, t.$emit("task-node-size", Object(tt["a"])({}, [t.taskUuid], s)))
                             }
                         })
                     }
                 }
             },
-            ge = he,
-            ye = (a("26ad"), Object(Rt["a"])(ge, se, ne, !1, null, "e080e642", null)),
-            me = ye.exports,
-            ke = {
+            ye = ge,
+            me = (a("e7c1"), Object(It["a"])(ye, ne, re, !1, null, "19c0b619", null)),
+            ke = me.exports,
+            ve = {
                 name: "XCollapseableTaskNode",
                 components: {
-                    XTaskNode: me
+                    XTaskNode: ke
                 },
                 props: {
                     taskUuid: {
                         required: !0
                     },
                     width: {
                         required: !0
                     },
                     height: {
                         required: !0
                     }
                 },
                 data: function() {
                     return {
-                        stackCount: ie
+                        stackCount: se
                     }
                 },
                 computed: {
                     descendantUuids: function() {
                         return this.$store.getters["graph/graphDataByUuid"][this.taskUuid].descendantUuids
                     },
                     collapseDetails: function() {
@@ -1498,21 +1504,21 @@
                     isLeaf: function() {
                         return this.$store.getters["graph/graphDataByUuid"][this.taskUuid].isLeaf
                     },
                     collapsedUuidsCount: function() {
                         return this.collapseDetails.collapsedUuids.length
                     },
                     areAllDescendantsCollapsed: function() {
-                        return Dt(this.collapseDetails.collapsedUuids, this.descendantUuids)
+                        return bt(this.collapseDetails.collapsedUuids, this.descendantUuids)
                     },
                     hasCollapsedChildren: function() {
                         return this.collapseDetails.collapsedUuids.length > 0
                     },
                     allStackOffset: function() {
-                        return ie * ae
+                        return se * ie
                     },
                     boxDimensions: function() {
                         var t = this.width - 2 * this.allStackOffset,
                             e = this.height - (this.hasCollapsedChildren ? this.allStackOffset : 0);
                         return {
                             width: t,
                             height: e
@@ -1531,33 +1537,33 @@
                         return {
                             width: "".concat(this.boxDimensions.width, "px"),
                             height: "".concat(this.boxDimensions.height, "px"),
                             display: "inline-block"
                         }
                     },
                     stacksContainerStyle: function() {
-                        var t = (ie - 1) * ae;
+                        var t = (se - 1) * ie;
                         return $.a.merge(this.getNonFrontBoxMargins(1), {
                             width: "".concat(this.boxDimensions.width + t, "px"),
                             height: "".concat(this.boxDimensions.height + t, "px")
                         })
                     }
                 },
                 methods: {
                     emitExpandUuids: function(t) {
-                        var e = St(t, "expand", "self", this.taskUuid);
-                        Nt.$emit("ui-collapse", {
+                        var e = _t(t, "expand", "self", this.taskUuid);
+                        Et.$emit("ui-collapse", {
                             keep_rel_pos_uuid: this.taskUuid,
                             operationsByUuid: e
                         })
                     },
                     getNonFrontBoxMargins: function(t) {
                         return {
-                            "margin-top": "".concat(ae * t, "px"),
-                            "margin-left": "".concat(ae * t, "px")
+                            "margin-top": "".concat(ie * t, "px"),
+                            "margin-left": "".concat(ie * t, "px")
                         }
                     },
                     getNonFrontBoxStyle: function(t) {
                         return $.a.merge(this.getNonFrontBoxMargins(t), {
                             background: this.collapseDetails.background,
                             "z-index": -(t + 1),
                             width: "".concat(this.boxDimensions.width, "px"),
@@ -1565,21 +1571,21 @@
                         })
                     },
                     expandAll: function() {
                         this.emitExpandUuids(this.collapseDetails.collapsedUuids)
                     }
                 }
             },
-            ve = ke,
-            Ae = (a("d005"), Object(Rt["a"])(ve, zt, Gt, !1, null, "4256192c", null)),
-            Ce = Ae.exports,
-            Ue = {
+            Ae = ve,
+            Ce = (a("d005"), Object(It["a"])(Ae, Vt, Gt, !1, null, "4256192c", null)),
+            Ue = Ce.exports,
+            xe = {
                 name: "XTaskSvgNodes",
                 components: {
-                    XCollapsableTaskNode: Ce
+                    XCollapsableTaskNode: Ue
                 },
                 props: {
                     nodeLayoutsByUuid: {
                         required: !0,
                         type: Object
                     }
                 },
@@ -1594,18 +1600,18 @@
                         return !$.a.isNull(this.focusedTaskUuid)
                     },
                     fadeTransitionName: function() {
                         return this.shouldFadeInNewNodes ? "fade" : null
                     }
                 }
             },
-            xe = Ue,
-            Se = (a("ee68"), Object(Rt["a"])(xe, Ht, Kt, !1, null, "4af60d56", null)),
-            _e = Se.exports,
-            Be = function() {
+            Se = xe,
+            _e = (a("ee68"), Object(It["a"])(Se, Kt, zt, !1, null, "4af60d56", null)),
+            Be = _e.exports,
+            De = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticStyle: {
                         overflow: "hidden",
                         width: "100%",
@@ -1631,19 +1637,19 @@
                         },
                         on: {
                             "task-node-size": t.receiveSize
                         }
                     })], 1)
                 }), 0)
             },
-            De = [],
-            be = {
+            be = [],
+            Te = {
                 name: "XSizeCapturingNodes",
                 components: {
-                    XTaskNode: me
+                    XTaskNode: ke
                 },
                 data: function() {
                     return {
                         sizesToCommit: {}
                     }
                 },
                 computed: {
@@ -1652,37 +1658,37 @@
                     },
                     allUuids: function() {
                         return this.$store.getters["tasks/allTaskUuids"]
                     }
                 },
                 methods: {
                     receiveSize: function(t) {
-                        $.a.isEmpty(this.dimensionsByUuid) ? (W()(this.sizesToCommit, t), Dt($.a.keys(this.sizesToCommit), this.allUuids) && (this.$store.dispatch("tasks/addTaskNodeSize", this.sizesToCommit), this.sizesToCommit = {})) : this.$store.dispatch("tasks/addTaskNodeSize", t)
+                        $.a.isEmpty(this.dimensionsByUuid) ? (W()(this.sizesToCommit, t), bt($.a.keys(this.sizesToCommit), this.allUuids) && (this.$store.dispatch("tasks/addTaskNodeSize", this.sizesToCommit), this.sizesToCommit = {})) : this.$store.dispatch("tasks/addTaskNodeSize", t)
                     }
                 }
             },
-            Te = be,
-            we = Object(Rt["a"])(Te, Be, De, !1, null, "8e547c5a", null),
-            Ne = we.exports,
-            Ee = function() {
+            we = Te,
+            Ne = Object(It["a"])(we, De, be, !1, null, "8e547c5a", null),
+            Ee = Ne.exports,
+            Oe = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("g", t._l(t.displayLinks, function(t) {
                     return a("path", {
                         key: t.id,
                         staticClass: "link",
                         attrs: {
                             d: t.d
                         }
                     })
                 }), 0)
             },
-            Oe = [],
-            Re = {
+            Re = [],
+            Ie = {
                 name: "XLinks",
                 props: {
                     parentUuidByUuid: {
                         required: !0,
                         type: Object
                     },
                     nodeLayoutsByUuid: {
@@ -1708,86 +1714,86 @@
                                     id: "".concat(s, "->").concat(i)
                                 })
                             }
                         }), e
                     }
                 }
             },
-            Ie = Re,
-            $e = (a("afa5"), Object(Rt["a"])(Ie, Ee, Oe, !1, null, "719e8d6a", null)),
-            Le = $e.exports,
+            $e = Ie,
+            Le = (a("afa5"), Object(It["a"])($e, Oe, Re, !1, null, "719e8d6a", null)),
+            Fe = Le.exports,
             Pe = a("f499"),
-            Fe = a.n(Pe);
+            Me = a.n(Pe);
 
-        function Me(t, e) {
+        function Qe(t, e) {
             try {
                 var a = JSON.parse(localStorage[t]);
                 return "*" === e ? a : $.a.pick(a, e)
             } catch (i) {
                 localStorage.removeItem(t)
             }
             return {}
         }
 
-        function Qe(t, e) {
-            var a = Me(t, "*"),
+        function Xe(t, e) {
+            var a = Qe(t, "*"),
                 i = $.a.assign(a, e);
-            localStorage[t] = Fe()(i)
+            localStorage[t] = Me()(i)
         }
 
-        function Xe(t, e, a) {
-            return $.a.get(Me(t, [e]), e, a)
+        function qe(t, e, a) {
+            return $.a.get(Qe(t, [e]), e, a)
         }
 
-        function qe(t) {
-            var e = Xe(t, "collapseConfig"),
+        function je(t) {
+            var e = qe(t, "collapseConfig"),
                 a = ["hideSuccessPaths", "uiCollapseOperationsByUuid", "applyDefaultCollapseOps"],
-                i = Dt($.a.keys(e), a),
+                i = bt($.a.keys(e), a),
                 s = $.a.every($.a.values($.a.get(e, "uiCollapseOperationsByUuid", {})), function(t) {
                     return $.a.every(t, function(t) {
-                        return Dt($.a.keys(t), ["operation", "priority", "targets", "sourceTaskUuid"])
+                        return bt($.a.keys(t), ["operation", "priority", "targets", "sourceTaskUuid"])
                     })
                 });
             return i && s ? e : {
                 uiCollapseOperationsByUuid: {},
                 hideSuccessPaths: !1,
                 applyDefaultCollapseOps: !0
             }
         }
 
-        function je() {
-            Nt.$emit("zoom", {
-                x: qt["b"].transform.x,
-                y: qt["b"].transform.y,
-                scale: qt["b"].transform.k
+        function He() {
+            Et.$emit("zoom", {
+                x: jt["b"].transform.x,
+                y: jt["b"].transform.y,
+                scale: jt["b"].transform.k
             })
         }
-        var He = {
+        var Ke = {
                 max: 2,
                 min: .05
             },
-            Ke = Object(Xt["a"])().scaleExtent([He.min, He.max]).clickDistance(4).on("zoom", je),
-            ze = {
+            ze = Object(qt["a"])().scaleExtent([Ke.min, Ke.max]).clickDistance(4).on("zoom", He),
+            Ve = {
                 name: "XGraph",
                 components: {
-                    XSvgTaskNodes: _e,
-                    XLink: Le,
-                    XTaskCapturingNodes: Ne
+                    XSvgTaskNodes: Be,
+                    XLink: Fe,
+                    XTaskCapturingNodes: Ee
                 },
                 data: function() {
                     return {
                         transform: {
                             x: 0,
                             y: 0,
                             scale: 1
                         },
                         nodeLayoutsByUuid: {}
                     }
                 },
-                computed: Object(Qt["a"])({}, Object(jt["c"])({
+                computed: Object(Xt["a"])({}, Object(Ht["c"])({
                     isFirstLayout: function(t) {
                         return t.graph.isFirstLayout
                     }
                 }), {
                     collapseConfig: function() {
                         return this.$store.state.graph.collapseConfig
                     },
@@ -1813,15 +1819,15 @@
                         return this.$store.state.tasks.taskNodeSizeByUuid
                     },
                     uncollapsedGraphByNodeUuid: function() {
                         return this.$store.getters["graph/uncollapsedGraphByNodeUuid"]
                     },
                     uncollapsedTaskNodeDimensionsByUuid: function() {
                         var t = this;
-                        if (this.isFirstLayout && !Dt($.a.keys(this.dimensionsByUuid), $.a.keys(this.uncollapsedGraphByNodeUuid))) return {};
+                        if (this.isFirstLayout && !bt($.a.keys(this.dimensionsByUuid), $.a.keys(this.uncollapsedGraphByNodeUuid))) return {};
                         var e = $.a.pick(this.uncollapsedGraphByNodeUuid, $.a.keys(this.dimensionsByUuid));
                         return $.a.mapValues(e, function(e, a) {
                             return $.a.merge({}, t.dimensionsByUuid[a], {
                                 uuid: a,
                                 width: t.dimensionsByUuid[a].width + e.widthPadding,
                                 height: t.dimensionsByUuid[a].height + e.heightPadding,
                                 parent_id: e.parent_id
@@ -1851,55 +1857,55 @@
                     },
                     uncollapsedNodeUuids: function() {
                         return this.$store.getters["graph/uncollapsedNodeUuids"]
                     },
                     allDescendantsCollapsedByUuid: function() {
                         var t = this;
                         return $.a.mapValues(this.uncollapsedGraphByNodeUuid, function(e, a) {
-                            return Dt(e.collapsedUuids, t.graphDataByUuid[a].descendantUuids)
+                            return bt(e.collapsedUuids, t.graphDataByUuid[a].descendantUuids)
                         })
                     },
                     focusedNodeUuid: function() {
                         return this.$store.state.tasks.focusedTaskUuid
                     }
                 }),
                 created: function() {
-                    Nt.$on("center", this.center), Nt.$on("ui-collapse", this.handleUiCollapseEvent), Nt.$on("toggle-task-collapse", this.toggleCollapseDescendants), Nt.$on("zoom", this.zoomed)
+                    Et.$on("center", this.center), Et.$on("ui-collapse", this.handleUiCollapseEvent), Et.$on("toggle-task-collapse", this.toggleCollapseDescendants), Et.$on("zoom", this.zoomed)
                 },
                 beforeDestroy: function() {
-                    Nt.$off("ui-collapse"), Nt.$off("toggle-task-collapse"), Nt.$off("zoom"), Nt.$off("center")
+                    Et.$off("ui-collapse"), Et.$off("toggle-task-collapse"), Et.$off("zoom"), Et.$off("center")
                 },
                 mounted: function() {
-                    Object(qt["f"])("div#chart-container").call(Ke).on("dblclick.zoom", null), this.$el.focus()
+                    Object(jt["f"])("div#chart-container").call(ze).on("dblclick.zoom", null), this.$el.focus()
                 },
                 methods: {
                     zoomed: function(t) {
-                        null !== qt["b"].sourceEvent && null !== this.focusedNodeUuid && this.$store.commit("tasks/setFocusedTaskUuid", null), this.transform = t, Qe(this.firexUid, this.transform)
+                        null !== jt["b"].sourceEvent && null !== this.focusedNodeUuid && this.$store.commit("tasks/setFocusedTaskUuid", null), this.transform = t, Xe(this.firexUid, this.transform)
                     },
                     updateTransformViaZoom: function(t) {
-                        var e = Xt["b"].translate(t.x, t.y).scale(t.scale);
-                        Object(qt["f"])("div#chart-container").call(Ke.transform, e)
+                        var e = qt["b"].translate(t.x, t.y).scale(t.scale);
+                        Object(jt["f"])("div#chart-container").call(ze.transform, e)
                     },
                     translateBy: function(t, e) {
-                        Object(qt["f"])("div#chart-container").call(Ke.translateBy, t, e)
+                        Object(jt["f"])("div#chart-container").call(ze.translateBy, t, e)
                     },
                     getCurrentRelPos: function(t) {
                         var e = this.nodeLayoutsByUuid[t];
                         return {
                             x: e.x + this.transform.x,
                             y: e.y + this.transform.y
                         }
                     },
                     center: function() {
                         this.updateTransformViaZoom(this.getCenterTransform())
                     },
                     getCenterTransform: function() {
                         if (this.$refs["graph-svg"]) {
                             var t = this.$refs["graph-svg"].getBoundingClientRect();
-                            if ($.a.every(this.nonCollapsedNodesExtent, $.a.negate($.a.isNil))) return dt(this.nonCollapsedNodesExtent, t, He, 200)
+                            if ($.a.every(this.nonCollapsedNodesExtent, $.a.negate($.a.isNil))) return dt(this.nonCollapsedNodesExtent, t, Ke, 200)
                         }
                         return {
                             x: 0,
                             y: 0,
                             scale: 1
                         }
                     },
@@ -1909,32 +1915,32 @@
                                 a = this.nodeLayoutsByUuid[t],
                                 i = {
                                     left: a.x,
                                     right: a.x + a.width,
                                     top: a.y,
                                     bottom: a.y + a.height
                                 };
-                            return dt(i, e, He, 0)
+                            return dt(i, e, Ke, 0)
                         }
                         return {
                             x: 0,
                             y: 0,
                             scale: 1
                         }
                     },
                     toggleCollapseDescendants: function(t) {
                         var e = this,
                             a = $.a.every(this.childrenUuidsByUuid[t], function(t) {
                                 return e.isCollapsedByUuid[t]
                             }),
                             i = this.allDescendantsCollapsedByUuid[t],
-                            s = Jt(t, i, a, this.collapseConfig.uiCollapseOperationsByUuid);
+                            s = Zt(t, i, a, this.collapseConfig.uiCollapseOperationsByUuid);
                         this.handleUiCollapseEvent({
                             keep_rel_pos_uuid: t,
-                            operationsByUuid: St(s.uuids, s.operation, s.target, t)
+                            operationsByUuid: _t(s.uuids, s.operation, s.target, t)
                         })
                     },
                     handleUiCollapseEvent: function(t) {
                         var e = this,
                             a = t.keep_rel_pos_uuid ? this.getCurrentRelPos(t.keep_rel_pos_uuid) : void 0,
                             i = $.a.mapValues(t.operationsByUuid, function(t, a) {
                                 var i, s = $.a.get(e.collapseConfig.uiCollapseOperationsByUuid, a, []);
@@ -1957,41 +1963,41 @@
                         if ($.a.isNil(t)) return !1;
                         var e = [t.x, t.y, t.scale];
                         return $.a.every($.a.map(e, function(t) {
                             return !$.a.isNil(t) && $.a.isNumber(t)
                         }))
                     },
                     getLocalStorageTransform: function() {
-                        var t = Me(this.firexUid, ["x", "y", "scale"]);
+                        var t = Qe(this.firexUid, ["x", "y", "scale"]);
                         return this.isTransformValid(t) ? t : this.getCenterTransform()
                     },
                     updateLayout: function() {
                         var t = this,
                             e = lt(this.uncollapsedTaskNodeDimensionsByUuid);
                         this.nodeLayoutsByUuid = R()($.a.mapValues(e, function(e, a) {
                             return $.a.assign(e, $.a.pick(t.uncollapsedTaskNodeDimensionsByUuid[a], "width", "height"))
                         }))
                     }
                 },
                 watch: {
                     firexUid: {
                         handler: function() {
-                            this.$store.commit("graph/setIsFirstLayout", !0), this.nodeLayoutsByUuid = {}, this.$store.commit("graph/setCollapseConfig", qe(this.firexUid))
+                            this.$store.commit("graph/setIsFirstLayout", !0), this.nodeLayoutsByUuid = {}, this.$store.commit("graph/setCollapseConfig", je(this.firexUid))
                         },
                         immediate: !0
                     },
                     nodeLayoutsByUuid: function(t) {
                         var e = this;
                         !$.a.isEmpty(t) && this.isFirstLayout && (this.$nextTick(function() {
                             return e.$store.commit("graph/setIsFirstLayout", !1)
                         }), this.updateTransformViaZoom(this.getLocalStorageTransform()))
                     },
                     collapseConfig: {
                         handler: function() {
-                            Qe(this.firexUid, {
+                            Xe(this.firexUid, {
                                 collapseConfig: this.collapseConfig
                             })
                         },
                         deep: !0
                     },
                     uncollapsedTaskNodeDimensionsByUuid: {
                         handler: function(t, e) {
@@ -2001,18 +2007,18 @@
                         immediate: !0
                     },
                     focusedNodeUuid: function(t) {
                         $.a.isNull(t) || this.updateTransformViaZoom(this.getCenterOnNodeTransform(t))
                     }
                 }
             },
-            Ge = ze,
-            Ve = (a("1723"), Object(Rt["a"])(Ge, Ft, Mt, !1, null, "7e9020b6", null)),
-            Ye = Ve.exports,
-            Je = function() {
+            Ge = Ve,
+            Ye = (a("1723"), Object(It["a"])(Ge, Mt, Qt, !1, null, "7e9020b6", null)),
+            Je = Ye.exports,
+            Ze = function() {
                 var t = this,
                     e = t.$createElement,
                     i = t._self._c || e;
                 return i("div", {
                     staticClass: "header"
                 }, [i("div", {
                     staticStyle: {
@@ -2050,80 +2056,100 @@
                         href: t.legacyUrl
                     }
                 }, [t._v("\n      🔥 Back to Legacy 🔥\n    ")]) : t._e(), i("div", {
                     staticStyle: {
                         "margin-left": "auto",
                         display: "flex"
                     }
-                }, [t._t("prebuttons"), t._l(t.links, function(e) {
-                    return [e.to ? i("popper", {
-                        key: e.name,
-                        staticClass: "flame-link",
+                }, [t._t("prebuttons"), t._l(t.links, function(t) {
+                    return [i("x-header-button", {
+                        key: t.name,
                         attrs: {
-                            trigger: "hover",
-                            options: {
-                                placement: "bottom"
-                            },
-                            disabled: !Boolean(e.title)
+                            link: t
                         }
-                    }, [i("div", {
-                        staticClass: "popper header-popover"
-                    }, [t._v(t._s(e.title))]), i("div", {
-                        attrs: {
-                            slot: "reference"
+                    })]
+                })], 2)])])
+            },
+            We = [],
+            ta = function() {
+                var t = this,
+                    e = t.$createElement,
+                    a = t._self._c || e;
+                return a("popper", {
+                    attrs: {
+                        trigger: "hover",
+                        options: {
+                            placement: "bottom"
                         },
+                        disabled: !Boolean(t.link.title)
+                    }
+                }, [a("div", {
+                    staticClass: "popper header-popover"
+                }, [t._v(t._s(t.link.title))]), a("div", {
+                    staticClass: "flame-link",
+                    attrs: {
                         slot: "reference"
-                    }, [i("router-link", {
-                        attrs: {
-                            to: e.to
-                        }
-                    }, [e.icon ? i("font-awesome-icon", {
-                        attrs: {
-                            icon: e.icon,
-                            "fixed-width": ""
-                        }
-                    }) : t._e(), e.text ? [t._v(t._s(e.text))] : t._e()], 2)], 1)]) : e.href ? i("a", {
-                        key: e.name,
-                        staticClass: "flame-link",
-                        attrs: {
-                            href: e.href
-                        }
-                    }, [e.icon ? i("font-awesome-icon", {
-                        attrs: {
-                            icon: e.icon,
-                            "fixed-width": ""
-                        }
-                    }) : t._e(), e.text ? [t._v(t._s(e.text))] : t._e()], 2) : e.on ? i("div", {
-                        key: e.name,
-                        staticClass: "header-icon-button",
-                        class: e._class,
-                        style: e.toggleState ? "color: #2B2;" : "",
-                        attrs: {
-                            title: e.title
-                        },
-                        on: {
-                            click: function(t) {
-                                return e.on()
-                            }
-                        }
-                    }, [e.icon ? i("font-awesome-icon", {
-                        attrs: {
-                            icon: e.icon,
-                            "fixed-width": ""
+                    },
+                    slot: "reference"
+                }, [t.link.to ? a("router-link", {
+                    attrs: {
+                        to: t.link.to
+                    }
+                }, [t.link.icon ? a("font-awesome-icon", {
+                    attrs: {
+                        icon: t.link.icon,
+                        "fixed-width": ""
+                    }
+                }) : t._e(), t.link.text ? [t._v(t._s(t.link.text))] : t._e()], 2) : t.link.href ? a("a", {
+                    attrs: {
+                        href: t.link.href
+                    }
+                }, [t.link.icon ? a("font-awesome-icon", {
+                    attrs: {
+                        icon: t.link.icon,
+                        "fixed-width": ""
+                    }
+                }) : t._e(), t.link.text ? [t._v(t._s(t.link.text))] : t._e()], 2) : t.link.on ? a("div", {
+                    staticClass: "header-icon-button",
+                    class: t.link._class,
+                    style: t.link.toggleState ? "color: #2B2;" : "",
+                    on: {
+                        click: function(e) {
+                            return t.link.on()
                         }
-                    }) : t._e(), e.text ? [t._v(t._s(e.text))] : t._e()], 2) : t._e()]
-                })], 2)])])
+                    }
+                }, [t.link.icon ? a("font-awesome-icon", {
+                    attrs: {
+                        icon: t.link.icon,
+                        "fixed-width": ""
+                    }
+                }) : t._e(), t.link.text ? [t._v(t._s(t.link.text))] : t._e()], 2) : t._e()], 1)])
             },
-            Ze = [],
-            We = a("526e"),
-            ta = a.n(We),
-            ea = (a("a101"), {
+            ea = [],
+            aa = a("526e"),
+            ia = a.n(aa),
+            sa = (a("a101"), {
+                name: "XHeaderButton",
+                components: {
+                    Popper: ia.a
+                },
+                props: {
+                    link: {
+                        required: !0,
+                        type: Object
+                    }
+                }
+            }),
+            na = sa,
+            ra = (a("b9fa"), Object(It["a"])(na, ta, ea, !1, null, null, null)),
+            oa = ra.exports,
+            ua = {
                 name: "XHeader",
                 components: {
-                    Popper: ta.a
+                    XHeaderButton: oa
                 },
                 props: {
                     title: {
                         default: ""
                     },
                     links: {
                         default: function() {
@@ -2131,15 +2157,15 @@
                         },
                         type: Array
                     },
                     legacyPath: {
                         default: ""
                     }
                 },
-                computed: Object(Qt["a"])({}, Object(jt["c"])({
+                computed: Object(Xt["a"])({}, Object(Ht["c"])({
                     chain: function(t) {
                         return t.firexRunMetadata.chain
                     },
                     centralServer: function(t) {
                         return t.firexRunMetadata.centralServer
                     }
                 }), {
@@ -2147,42 +2173,32 @@
                         var t = $.a.get(this.$route, "query.flameServer", "");
                         return "".concat(t).concat(this.legacyPath, "?noUpgrade=true")
                     },
                     isCiscoDeployment: function() {
                         return "http://firex.cisco.com" === this.centralServer
                     }
                 })
-            }),
-            aa = ea,
-            ia = (a("e153"), Object(Rt["a"])(aa, Je, Ze, !1, null, "061bf61e", null)),
-            sa = ia.exports,
-            na = function() {
+            },
+            la = ua,
+            ca = (a("78a6"), Object(It["a"])(la, Ze, We, !1, null, "5a00c5be", null)),
+            da = ca.exports,
+            pa = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticStyle: {
-                        "border-left": "1px solid #000",
-                        padding: "0 8px"
-                    }
-                }, [a("span", {
-                    staticClass: "collapse-button",
-                    attrs: {
-                        title: "Expand All"
-                    },
-                    on: {
-                        click: function(e) {
-                            return t.dispatchCollapseAction("graph/expandAll")
-                        }
+                        "padding-right": "8px",
+                        display: "flex"
                     }
-                }, [a("font-awesome-icon", {
+                }, [a("x-header-button", {
                     attrs: {
-                        icon: "expand-arrows-alt"
+                        link: t.expandAllLink
                     }
-                })], 1), t.anyCollapseOptionsAvailable ? a("popper", {
+                }), t.anyCollapseOptionsAvailable ? a("popper", {
                     attrs: {
                         trigger: "hover",
                         options: {
                             placement: "bottom"
                         },
                         disabled: t.dropDownDisabled
                     }
@@ -2235,30 +2251,31 @@
                     slot: "reference"
                 }, [a("font-awesome-icon", {
                     attrs: {
                         icon: "caret-down"
                     }
                 })], 1)]) : t._e()], 1)
             },
-            ra = [],
-            oa = {
+            fa = [],
+            ha = {
                 name: "XCollapseButtons",
                 components: {
-                    Popper: ta.a
+                    XHeaderButton: oa,
+                    Popper: ia.a
                 },
                 data: function() {
                     return {
                         dropDownDisabled: !1
                     }
                 },
-                computed: Object(Qt["a"])({}, Object(jt["c"])({
+                computed: Object(Xt["a"])({}, Object(Ht["c"])({
                     collapseConfig: function(t) {
                         return t.graph.collapseConfig
                     }
-                }), Object(jt["b"])({
+                }), Object(Ht["b"])({
                     collapsedNodeUuids: "graph/collapsedNodeUuids",
                     userDisplayConfigOperationsByUuid: "graph/userDisplayConfigOperationsByUuid",
                     flameDataDisplayOperationsByUuid: "graph/flameDataDisplayOperationsByUuid",
                     runStateByUuid: "tasks/runStateByUuid"
                 }), {
                     hasCollapsedNodes: function() {
                         return this.collapsedNodeUuids.length > 0
@@ -2275,41 +2292,53 @@
                     },
                     hasFailures: function() {
                         return $.a.some($.a.values(this.runStateByUuid), {
                             state: "task-failed"
                         })
                     },
                     anyCollapseOptionsAvailable: function() {
-                        return this.hasCollapsedNodes || this.canRestoreDefault || this.canShowOnlyFailed
+                        return this.canRestoreDefault || this.canShowOnlyFailed
+                    },
+                    expandAllLink: function() {
+                        var t = this;
+                        return {
+                            on: function() {
+                                t.dispatchCollapseAction("graph/expandAll")
+                            },
+                            title: "Expand All",
+                            icon: "expand-arrows-alt"
+                        }
                     }
                 }),
                 methods: {
                     dispatchCollapseAction: function(t) {
                         this.$store.dispatch(t), this.$nextTick(function() {
-                            Nt.$emit("center")
+                            Et.$emit("center")
                         })
                     },
                     toggleDropdownDisabled: function() {
                         var t = this;
                         this.dropDownDisabled = !0, this.$nextTick(function() {
                             t.dropDownDisabled = !1
                         })
                     }
                 }
             },
-            ua = oa,
-            la = (a("9b2d"), Object(Rt["a"])(ua, na, ra, !1, null, "0de53894", null)),
-            ca = la.exports,
-            da = function() {
+            ga = ha,
+            ya = (a("2638"), Object(It["a"])(ga, pa, fa, !1, null, "ac58f39e", null)),
+            ma = ya.exports,
+            ka = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticStyle: {
-                        display: "flex"
+                        display: "flex",
+                        border: "none",
+                        "border-left": "1px solid #000"
                     }
                 }, [t.searchOpen ? a("div", {
                     on: {
                         keydown: function(e) {
                             return !e.type.indexOf("key") && t._k(e.keyCode, "esc", 27, e.key, ["Esc", "Escape"]) ? null : t.$store.commit("tasks/closeSearch")
                         }
                     }
@@ -2331,55 +2360,58 @@
                     on: {
                         keyup: [function(e) {
                             return !e.type.indexOf("key") && t._k(e.keyCode, "enter", 13, e.key, "Enter") ? null : e.ctrlKey || e.shiftKey || e.altKey || e.metaKey ? null : void t.submitSearch(e.target.value.trim())
                         }, function(e) {
                             return !e.type.indexOf("key") && t._k(e.keyCode, "enter", 13, e.key, "Enter") ? null : e.shiftKey ? t.$store.dispatch("tasks/previousSearchResult") : null
                         }]
                     }
-                })]) : t._e(), a("div", {
-                    staticClass: "header-icon-button",
+                })]) : t._e(), a("x-header-button", {
                     style: t.searchOpen ? "color: #2B2;" : "",
                     attrs: {
-                        title: "Search"
-                    },
-                    on: {
-                        click: function(e) {
-                            return t.$store.commit("tasks/toggleSearchOpen")
-                        }
-                    }
-                }, [a("font-awesome-icon", {
-                    attrs: {
-                        icon: "search",
-                        "fixed-width": ""
+                        link: t.buttonLink
                     }
-                })], 1)])
+                })], 1)
             },
-            pa = [],
-            fa = (a("386d"), {
+            va = [],
+            Aa = (a("386d"), {
                 name: "XTaskNodeSearch",
+                components: {
+                    XHeaderButton: oa
+                },
                 props: {
                     findUncollapsedAncestor: {
                         default: !0,
                         type: Boolean
                     }
                 },
-                computed: Object(Qt["a"])({}, Object(jt["c"])({
+                computed: Object(Xt["a"])({}, Object(Ht["c"])({
                     selectedIndex: function(t) {
                         return t.tasks.search.selectedIndex
                     },
                     searchResultCount: function(t) {
                         return t.tasks.search.resultUuids.length
                     },
                     searchOpen: function(t) {
                         return t.tasks.search.isOpen
                     },
                     searchTerm: function(t) {
                         return t.tasks.search.term
                     }
-                })),
+                }), {
+                    buttonLink: function() {
+                        var t = this;
+                        return {
+                            on: function() {
+                                t.$store.commit("tasks/toggleSearchOpen")
+                            },
+                            icon: "search",
+                            title: "Search"
+                        }
+                    }
+                }),
                 methods: {
                     submitSearch: function(t) {
                         this.$store.dispatch("tasks/search", {
                             term: t,
                             findUncollapsedAncestor: this.findUncollapsedAncestor
                         })
                     }
@@ -2389,24 +2421,24 @@
                         var e = this;
                         t && this.$nextTick(function() {
                             e.$refs["search-input"].focus()
                         })
                     }
                 }
             }),
-            ha = fa,
-            ga = (a("52f7"), Object(Rt["a"])(ha, da, pa, !1, null, "409babf4", null)),
-            ya = ga.exports,
-            ma = {
+            Ca = Aa,
+            Ua = (a("177d"), Object(It["a"])(Ca, ka, va, !1, null, "6ee28668", null)),
+            xa = Ua.exports,
+            Sa = {
                 name: "XHeaderedGraph",
                 components: {
-                    XGraph: Ye,
-                    XHeader: sa,
-                    XCollapseButtons: ca,
-                    XTaskNodeSearch: ya
+                    XGraph: Je,
+                    XHeader: da,
+                    XCollapseButtons: ma,
+                    XTaskNodeSearch: xa
                 },
                 props: {
                     rootUuid: {
                         default: null
                     }
                 },
                 computed: {
@@ -2430,15 +2462,15 @@
                                     return t.$store.dispatch("graph/toggleLiveUpdate")
                                 },
                                 toggleState: this.toggleStates.liveUpdate,
                                 icon: ["far", "eye"]
                             }, {
                                 name: "center",
                                 on: function() {
-                                    return Nt.$emit("center")
+                                    return Et.$emit("center")
                                 },
                                 icon: "bullseye",
                                 title: "Center"
                             }, {
                                 name: "showTaskDetails",
                                 on: function() {
                                     return t.$store.dispatch("graph/toggleShowTaskDetails")
@@ -2455,15 +2487,15 @@
                                 name: "time-chart",
                                 to: ct(this.$route.query, "XTimeChart"),
                                 icon: "clock",
                                 title: "Time Chart"
                             }, {
                                 name: "kill",
                                 on: function() {
-                                    return Nt.$emit("revoke-root")
+                                    return Et.$emit("revoke-root")
                                 },
                                 _class: "kill-button",
                                 icon: "times",
                                 title: "Kill"
                             }, {
                                 name: "logs",
                                 href: this.$store.getters["firexRunMetadata/logsUrl"],
@@ -2485,32 +2517,32 @@
                     }
                 },
                 methods: {
                     focusOnFind: function() {
                         this.$store.commit("tasks/toggleSearchOpen")
                     },
                     refreshGraph: function() {
-                        Nt.$emit("graph-refresh")
+                        Et.$emit("graph-refresh")
                     }
                 },
                 watch: {
                     rootUuid: {
                         handler: function() {
                             null !== this.rootUuid && this.$nextTick(function() {
-                                Nt.$emit("center")
+                                Et.$emit("center")
                             }), this.$store.dispatch("tasks/selectRootUuid", this.rootUuid)
                         },
                         immediate: !0
                     }
                 }
             },
-            ka = ma,
-            va = Object(Rt["a"])(ka, Lt, Pt, !1, null, "495f7ec8", null),
-            Aa = va.exports,
-            Ca = function() {
+            _a = Sa,
+            Ba = Object(It["a"])(_a, Ft, Pt, !1, null, "ddc3bc26", null),
+            Da = Ba.exports,
+            ba = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticStyle: {
                         width: "100%",
                         height: "100%",
@@ -2535,15 +2567,14 @@
                         links: t.headerLinks,
                         legacyPath: "/list"
                     },
                     scopedSlots: t._u([{
                         key: "prebuttons",
                         fn: function() {
                             return [a("x-task-node-search", {
-                                staticClass: "header-icon-button",
                                 attrs: {
                                     findUncollapsedAncestor: !1
                                 }
                             })]
                         },
                         proxy: !0
                     }])
@@ -2727,26 +2758,26 @@
                         attrs: {
                             taskUuid: t,
                             isLeaf: !0
                         }
                     })
                 }), 1)])], 1)
             },
-            Ua = [function() {
+            Ta = [function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", [a("hr")])
             }],
-            xa = (a("55dd"), {
+            wa = (a("55dd"), {
                 name: "XList",
                 components: {
-                    XNode: me,
-                    XHeader: sa,
-                    XTaskNodeSearch: ya
+                    XNode: ke,
+                    XHeader: da,
+                    XTaskNodeSearch: xa
                 },
                 props: {
                     sort: {
                         required: !0,
                         type: String
                     },
                     sortDirection: {
@@ -2783,15 +2814,15 @@
                         }, {
                             value: "runtime",
                             text: "Runtime"
                         }],
                         runStateSelectorsToStates: t
                     }
                 },
-                computed: Object(Qt["a"])({}, Object(jt["c"])({
+                computed: Object(Xt["a"])({}, Object(Ht["c"])({
                     allTasksByUuid: function(t) {
                         return t.tasks.allTasksByUuid
                     },
                     search: function(t) {
                         return t.tasks.search
                     }
                 }), {
@@ -2807,24 +2838,26 @@
                     title: function() {
                         return this.$store.state.firexRunMetadata.uid
                     },
                     headerLinks: function() {
                         return [{
                             name: "graph",
                             to: ct(this.$route.query, "XGraph"),
-                            icon: "sitemap"
+                            icon: "sitemap",
+                            title: "Main Graph"
                         }, {
                             name: "logs",
                             href: this.$store.getters["firexRunMetadata/logsUrl"],
                             text: "Logs",
                             icon: "file-alt"
                         }, {
                             name: "help",
                             to: ct(this.$route.query, "XHelp"),
-                            text: "Help"
+                            text: "Help",
+                            icon: "question-circle"
                         }]
                     },
                     sortedTasksUuids: function() {
                         var t = {
                                 "time-received": "task_num",
                                 alphabetical: "name",
                                 runtime: "actual_runtime"
@@ -2843,15 +2876,15 @@
                     displayTaskUuids: function() {
                         return $.a.intersection(this.sortedTasksUuids, this.filteredTaskUuids)
                     },
                     selectedRunStates: function() {
                         return $.a.flatten($.a.values($.a.pick(this.runStateSelectorsToStates, this.selectedOptions.runStates)))
                     },
                     allRunStatesSelected: function() {
-                        return Dt(this.selectedRunStates, this.allRunStates)
+                        return bt(this.selectedRunStates, this.allRunStates)
                     },
                     allRunStates: function() {
                         return $.a.uniq($.a.flatten($.a.values(this.runStateSelectorsToStates)))
                     }
                 }),
                 methods: {
                     toggleShowAll: function() {
@@ -2908,18 +2941,18 @@
                                 return e.updateRouteQuery(t.key, t.value)
                             })
                         },
                         deep: !0
                     }
                 }
             }),
-            Sa = xa,
-            _a = (a("65cf"), Object(Rt["a"])(Sa, Ca, Ua, !1, null, "2470f47c", null)),
-            Ba = _a.exports,
-            Da = function() {
+            Na = wa,
+            Ea = (a("8d0f"), Object(It["a"])(Na, ba, Ta, !1, null, "d2e6a2bc", null)),
+            Oa = Ea.exports,
+            Ra = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     ref: "time-table",
                     staticStyle: {
                         width: "100%",
@@ -2945,15 +2978,14 @@
                         links: t.headerLinks,
                         legacyPath: "/list"
                     },
                     scopedSlots: t._u([{
                         key: "prebuttons",
                         fn: function() {
                             return [a("x-task-node-search", {
-                                staticClass: "header-icon-button",
                                 attrs: {
                                     findUncollapsedAncestor: !1
                                 }
                             })]
                         },
                         proxy: !0
                     }])
@@ -3051,52 +3083,108 @@
                         key: e.uuid
                     }, [a("td", {
                         staticClass: "min"
                     }, [t._v(t._s(e.task_num))]), a("td", {
                         staticClass: "min"
                     }, [t._v(t._s(e.name))]), a("td", {
                         staticClass: "min"
-                    }, [t._v(t._s(e.hostname))]), a("td", [a("popper", {
+                    }, [t._v(t._s(e.hostname))]), a("td", [a("div", {
+                        staticStyle: {
+                            display: "flex",
+                            "flex-direction": "column",
+                            height: "1.5em"
+                        },
+                        style: t.taskRectOffsetStyleByUuid[e.uuid]
+                    }, [a("div", {
+                        staticStyle: {
+                            height: "0.75em",
+                            display: "flex",
+                            "flex-direction": "row"
+                        }
+                    }, t._l(t.perStateRectByUuid[e.uuid], function(i, s) {
+                        return a("div", {
+                            key: s,
+                            staticClass: "state-rect",
+                            style: i
+                        }, [a("popper", {
+                            staticStyle: {
+                                display: "block"
+                            },
+                            attrs: {
+                                trigger: "hover",
+                                options: {
+                                    placement: "top"
+                                }
+                            }
+                        }, [a("div", {
+                            staticClass: "popper popover-container"
+                        }, [a("div", {
+                            staticClass: "popover-title"
+                        }, [a("b", [t._v(t._s(e.name))])]), a("div", {
+                            staticStyle: {
+                                padding: "3px"
+                            }
+                        }, [t._v("\n                      " + t._s(t.getRunstateDisplayName(i.state)) + " at\n                      " + t._s(t.formatShortTime(i.timestamp, t.shortTimeSec)) + "\n                    ")]), a("div", {
+                            staticStyle: {
+                                padding: "3px"
+                            }
+                        }, [t._v("\n                      " + t._s(t.getRunstateDisplayName(i.state)) + "\n                      for " + t._s(t.durationString(i.stateDuraion)) + "\n                      (" + t._s((100 * i.stateDuraion / t.displayTasksDuration).toFixed(2)) + "% of run)\n                    ")])]), a("span", {
+                            staticStyle: {
+                                display: "block",
+                                height: "0.75em"
+                            },
+                            attrs: {
+                                slot: "reference"
+                            },
+                            slot: "reference"
+                        })])], 1)
+                    }), 0), t.isTaskStateIncomplete(e.state) ? t._e() : a("div", {
+                        staticStyle: {
+                            display: "block",
+                            height: "0.75em"
+                        }
+                    }, [a("popper", {
                         attrs: {
                             trigger: "hover",
                             options: {
-                                placement: "top"
+                                placement: "bottom"
                             }
                         }
                     }, [a("div", {
                         staticClass: "popper popover-container"
                     }, [a("div", {
                         staticClass: "popover-title"
                     }, [a("b", [t._v(t._s(e.name))])]), a("div", {
                         staticStyle: {
                             padding: "3px"
                         }
-                    }, [t._v("\n                  Started: " + t._s(t.formatShortTime(e.first_started, t.shortTimeSec)) + "\n                ")]), a("div", {
+                    }, [t._v("\n                      Started: " + t._s(t.formatShortTime(e.first_started, t.shortTimeSec)) + "\n                    ")]), a("div", {
                         staticStyle: {
                             padding: "3px"
                         }
-                    }, [t._v("\n                  Runtime: " + t._s(t.durationString(t.getRuntime(e))) + "\n                  (" + t._s((100 * t.getRuntime(e) / t.displayTasksDuration).toFixed(2)) + "%)\n                ")])]), a("div", {
+                    }, [t._v("\n                      Runtime: " + t._s(t.durationString(t.getRuntime(e))) + "\n                      (" + t._s((100 * t.getRuntime(e) / t.displayTasksDuration).toFixed(2)) + "%)\n                    ")])]), a("span", {
                         staticStyle: {
-                            height: "1em"
+                            height: "0.75em",
+                            display: "block"
                         },
-                        style: t.chartRectStyleByUuid[e.uuid],
+                        style: t.fullTaskRectStyleByUuid[e.uuid],
                         attrs: {
                             slot: "reference"
                         },
                         slot: "reference"
                     }, [a("router-link", {
                         staticClass: "task",
                         staticStyle: {
                             display: "block",
                             height: "100%"
                         },
                         attrs: {
                             to: t.routeToAttribute(e.uuid)
                         }
-                    })], 1)])], 1), a("td", {
+                    })], 1)])], 1)])]), a("td", {
                         staticClass: "min"
                     }, [e.uuid in t.extraTaskFieldsByUuid ? a("div", {
                         staticClass: "icon-links"
                     }, [a("a", {
                         attrs: {
                             href: t.extraTaskFieldsByUuid[e.uuid].logs_url,
                             title: "logs"
@@ -3122,22 +3210,22 @@
                     }, [a("font-awesome-icon", {
                         attrs: {
                             icon: "file-code"
                         }
                     })], 1)], 1) : t._e()])])
                 }), 0)])])], 1)
             },
-            ba = [],
-            Ta = a("1315"),
-            wa = {
+            Ia = [],
+            $a = a("1315"),
+            La = {
                 name: "XTimeChart",
                 components: {
-                    XHeader: sa,
-                    XTaskNodeSearch: ya,
-                    Popper: ta.a
+                    XHeader: da,
+                    XTaskNodeSearch: xa,
+                    Popper: ia.a
                 },
                 props: {
                     sort: {
                         required: !0
                     },
                     sortDirection: {
                         required: !0
@@ -3154,15 +3242,15 @@
                         shortTime: t,
                         shortTimeSec: W()({
                             second: "2-digit"
                         }, t),
                         extraTaskFieldsByUuid: {}
                     }
                 },
-                computed: Object(Qt["a"])({}, Object(jt["c"])({
+                computed: Object(Xt["a"])({}, Object(Ht["c"])({
                     allTasksByUuid: function(t) {
                         return t.tasks.allTasksByUuid
                     },
                     title: function(t) {
                         return t.firexRunMetadata.uid
                     },
                     search: function(t) {
@@ -3183,19 +3271,21 @@
                         var e = $.a.sortBy(t, this.sort);
                         return "desc" === this.sortDirection && (e = $.a.reverse(e)), $.a.keyBy(e, "uuid")
                     },
                     headerLinks: function() {
                         return [{
                             name: "graph",
                             to: ct(this.$route.query, "XGraph"),
-                            icon: "sitemap"
+                            icon: "sitemap",
+                            title: "Main Graph"
                         }, {
                             name: "list",
                             to: ct(this.$route.query, "XList"),
-                            icon: "list-ul"
+                            icon: "list-ul",
+                            title: "List View"
                         }, {
                             name: "logs",
                             href: this.$store.getters["firexRunMetadata/logsUrl"],
                             text: "Logs",
                             icon: "file-alt"
                         }, {
                             name: "help",
@@ -3212,59 +3302,100 @@
                         return $.a.max($.a.map(this.displayTasks, function(e) {
                             return e.first_started + t.getRuntime(e)
                         }))
                     },
                     displayTasksDuration: function() {
                         return this.displayTasksEndTime - this.displayTasksStartTime
                     },
-                    chartRectByUuid: function() {
+                    fullTaskRectByUuid: function() {
                         var t = this;
                         return $.a.mapValues(this.displayTasks, function(e) {
                             var a = (e.first_started - t.displayTasksStartTime) / t.displayTasksDuration,
                                 i = t.getRuntime(e) / t.displayTasksDuration;
                             return {
                                 offset: 100 * a,
                                 duration: $.a.max([100 * i, .5])
                             }
                         })
                     },
-                    chartRectStyleByUuid: function() {
+                    perStateRectsByUuid: function() {
+                        var t = this;
+                        return $.a.mapValues(this.displayTasks, function(e, a) {
+                            return $.a.map($.a.get(t.extraTaskFieldsByUuid, [a, "states"], []), function(e, a, i) {
+                                var s = e.timestamp - t.displayTasksStartTime,
+                                    n = s / t.displayTasksDuration,
+                                    r = $.a.get(i, a + 1, {
+                                        timestamp: n
+                                    }),
+                                    o = r.timestamp - e.timestamp,
+                                    u = o / t.displayTasksDuration;
+                                return {
+                                    offset: 100 * n,
+                                    duration: 100 * u,
+                                    state: e.state,
+                                    timestamp: e.timestamp
+                                }
+                            })
+                        })
+                    },
+                    taskRectOffsetStyleByUuid: function() {
+                        var t = this;
+                        return $.a.mapValues(this.displayTasks, function(e) {
+                            return {
+                                "padding-left": "".concat(t.fullTaskRectByUuid[e.uuid].offset, "%")
+                            }
+                        })
+                    },
+                    fullTaskRectStyleByUuid: function() {
                         var t = this;
                         return $.a.mapValues(this.displayTasks, function(e) {
                             return {
-                                "margin-left": "".concat(t.chartRectByUuid[e.uuid].offset, "%"),
-                                width: "".concat(t.chartRectByUuid[e.uuid].duration, "%"),
+                                width: "".concat(t.fullTaskRectByUuid[e.uuid].duration, "%"),
                                 background: At(e.exception, e.state)
                             }
                         })
                     },
+                    perStateRectByUuid: function() {
+                        var t = this;
+                        return $.a.mapValues(this.perStateRectsByUuid, function(e, a) {
+                            return $.a.map(e, function(e) {
+                                return {
+                                    width: "".concat(e.duration, "%"),
+                                    background: At(t.displayTasks[a].exception, e.state),
+                                    state: e.state,
+                                    timestamp: e.timestamp,
+                                    stateDuraion: e.duration
+                                }
+                            })
+                        })
+                    },
                     isAsc: function() {
                         return "asc" === this.sortDirection
                     }
                 }),
                 created: function() {
                     var t = this;
-                    G(["states", "logs_url", "code_url"]).then(function(e) {
+                    V(["states", "logs_url", "code_url"]).then(function(e) {
                         t.extraTaskFieldsByUuid = e
                     })
                 },
                 methods: {
                     getRuntime: function(t) {
-                        if (pt(t.state)) return le()() / 1e3 - t.first_started;
+                        if (pt(t.state)) return ce()() / 1e3 - t.first_started;
                         if ($.a.has(t, "actual_runtime")) return t.actual_runtime;
                         var e = $.a.max($.a.map(this.allTasksByUuid, function(t) {
                             return t.first_started + $.a.get(t, "actual_runtime", 0)
                         }));
                         return e - t.first_started
                     },
                     formatTime: function(t) {
-                        return Ta["DateTime"].fromSeconds(t).toLocaleString(Ta["DateTime"].DATETIME_FULL)
+                        return $a["DateTime"].fromSeconds(t).toLocaleString($a["DateTime"].DATETIME_FULL)
                     },
                     formatShortTime: function(t, e) {
-                        return Ta["DateTime"].fromSeconds(t).toLocaleString(e)
+                        return $a["DateTime"].fromSeconds(t).toLocaleString(e)
                     },
                     routeToAttribute: function(t) {
                         return ct(this.$route.query, "XNodeAttributes", {
                             uuid: t
                         })
                     },
                     durationString: gt,
@@ -3282,29 +3413,31 @@
                             sortDirection: "asc"
                         })
                     },
                     rootRoute: function(t) {
                         return ct(this.$route.query, "custom-root", {
                             rootUuid: t
                         })
-                    }
+                    },
+                    getRunstateDisplayName: Ut,
+                    isTaskStateIncomplete: pt
                 },
                 beforeRouteLeave: function(t, e, a) {
                     e.meta.scrollY = this.$refs["time-table"].scrollTop, this.$store.commit("tasks/closeSearch"), a()
                 },
                 beforeRouteEnter: function(t, e, a) {
                     a(function(e) {
                         $.a.has(t.meta, "scrollY") && (e.$refs["time-table"].scrollTop = t.meta.scrollY, delete t.meta.scrollY)
                     })
                 }
             },
-            Na = wa,
-            Ea = (a("ab9b"), Object(Rt["a"])(Na, Da, ba, !1, null, "65363fc0", null)),
-            Oa = Ea.exports,
-            Ra = function() {
+            Fa = La,
+            Pa = (a("7a4d"), Object(It["a"])(Fa, Ra, Ia, !1, null, "53a20b2c", null)),
+            Ma = Pa.exports,
+            Qa = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticStyle: {
                         width: "100%",
                         height: "100%",
@@ -3392,19 +3525,19 @@
                             staticStyle: {
                                 margin: "0 0 0 40px"
                             }
                         }, [t._v(t._s(t.prettyPrint(e)))]) : [t._v(t._s(null === e ? "None" : e))]], 2)
                     }), 0) : a("span", [t._v("\n        " + t._s(t.displayKeyNode[e]) + "\n      ")])])
                 }), 0)], 1)
             },
-            Ia = [],
-            $a = {
+            Xa = [],
+            qa = {
                 name: "XNodeAttributes",
                 components: {
-                    XHeader: sa
+                    XHeader: da
                 },
                 props: {
                     uuid: {
                         required: !0,
                         type: String
                     }
                 },
@@ -3478,30 +3611,31 @@
                                 },
                                 toggleState: this.showAllAttributes,
                                 icon: "plus-circle",
                                 title: "Show All Attributes"
                             }, {
                                 name: "code",
                                 href: this.detailedTask.code_url,
-                                icon: "file-code"
+                                icon: "file-code",
+                                title: "See Code"
                             }, {
                                 name: "logs",
                                 href: this.detailedTask.logs_url,
                                 text: "Logs",
                                 icon: "file-alt"
                             }, {
                                 name: "support",
                                 href: this.detailedTask.support_location,
                                 text: "Support",
                                 icon: "question-circle"
                             }];
                         return pt(this.simpleTask.state) && (e = [{
                             name: "kill",
                             on: function() {
-                                return Nt.$emit("revoke-task", t.uuid)
+                                return Et.$emit("revoke-task", t.uuid)
                             },
                             _class: "kill-button",
                             icon: "times"
                         }].concat(e)), {
                             title: this.detailedTask.long_name,
                             legacyPath: "/task/".concat(this.uuid),
                             links: e
@@ -3521,41 +3655,41 @@
                         })
                     },
                     isObject: function(t) {
                         return $.a.isObject(t)
                     },
                     shouldPrettyPrint: function(t) {
                         if (!$.a.isObject(t)) return !1;
-                        var e = Fe()(t, null, 2);
+                        var e = Me()(t, null, 2);
                         return e.length > 100
                     },
                     prettyPrint: function(t) {
                         if (null === t) return "None";
-                        var e = Fe()(t, null, 2);
-                        return e.length < 40 ? Fe()(t) : e
+                        var e = Me()(t, null, 2);
+                        return e.length < 40 ? Me()(t) : e
                     },
                     isTimeKey: function(t) {
                         return $.a.includes(["first_started", "started", "failed", "succeeded", "revoked", "timestamp"], t)
                     },
                     formatTime: function(t) {
-                        var e = Ta["DateTime"].fromSeconds(t).toLocaleString(Ta["DateTime"].DATETIME_FULL);
+                        var e = $a["DateTime"].fromSeconds(t).toLocaleString($a["DateTime"].DATETIME_FULL);
                         return "".concat(e, " (orig: ").concat(t, ")")
                     }
                 },
                 watch: {
                     $route: {
                         handler: "fetchTaskAttributes",
                         immediate: !0
                     }
                 }
             },
-            La = $a,
-            Pa = (a("16c8"), Object(Rt["a"])(La, Ra, Ia, !1, null, "39c046bc", null)),
-            Fa = Pa.exports,
-            Ma = function() {
+            ja = qa,
+            Ha = (a("7071"), Object(It["a"])(ja, Qa, Xa, !1, null, "192505f8", null)),
+            Ka = Ha.exports,
+            za = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticStyle: {
                         width: "100%",
                         height: "100%",
@@ -3675,33 +3809,33 @@
                     attrs: {
                         taskUuid: "pluginSucceededNode",
                         "allow-click-to-attributes": !1,
                         isLeaf: !0
                     }
                 })], 1)])]), a("h1", [t._v("Difference between round and square corners")]), t._m(0)])], 1)
             },
-            Qa = [function() {
+            Va = [function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", [a("ul", [a("li", [a("h2", {
                     staticStyle: {
                         "font-weight": "normal"
                     }
                 }, [t._v("Round cornered tasks are tasks which are spawned\n            from within another task. The task which spawns them\n            appears as their parent. These tasks can be the root of a larger chain.")])]), a("li", [a("h2", {
                     staticStyle: {
                         "font-weight": "normal"
                     }
                 }, [t._v("Square cornered tasks are tasks which are chained\n            behind another task. The task which they are chained\n            with (or precedes them) appears as their parent. The root of a chain\n            will always have round corners.")])])])])
             }],
-            Xa = {
+            Ga = {
                 name: "XHelp",
                 components: {
-                    XHeader: sa,
-                    XNode: me
+                    XHeader: da,
+                    XNode: ke
                 },
                 data: function() {
                     return {
                         baseNode: {
                             name: "noop",
                             hostname: "hostname",
                             task_num: 1,
@@ -3730,15 +3864,15 @@
                         pluginSucceededNode: $.a.merge({}, this.baseNode, {
                             state: "task-succeeded",
                             from_plugin: !0
                         })
                     };
                     this.$store.dispatch("tasks/setTasks", t)
                 },
-                computed: Object(Qt["a"])({}, Object(jt["c"])({
+                computed: Object(Xt["a"])({}, Object(Ht["c"])({
                     docUrl: function(t) {
                         return t.firexRunMetadata.central_documentation_url
                     }
                 }), {
                     tasksByUuid: function() {
                         return {
                             startedNode: $.a.merge({}, this.baseNode, {
@@ -3785,18 +3919,18 @@
                         immediate: !0,
                         handler: function() {
                             this.$store.dispatch("tasks/setTasks", this.tasksByUuid)
                         }
                     }
                 }
             },
-            qa = Xa,
-            ja = (a("4e67"), Object(Rt["a"])(qa, Ma, Qa, !1, null, "6453f82e", null)),
-            Ha = ja.exports,
-            Ka = function() {
+            Ya = Ga,
+            Ja = (a("4e67"), Object(It["a"])(Ya, za, Va, !1, null, "6453f82e", null)),
+            Za = Ja.exports,
+            Wa = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticClass: "settings"
                 }, [a("h1", [t._v("Settings")]), a("div", {
                     staticStyle: {
@@ -4128,37 +4262,37 @@
                     }
                 }, [t._v("\n      " + t._s(t.displayConfigError) + "\n    ")]), a("button", {
                     on: {
                         click: t.saveDisplayConfigEntry
                     }
                 }, [t._v("Save Display Config")])])])
             },
-            za = [function() {
+            ti = [function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("thead", [a("tr", [a("td", [t._v("Service Name")]), a("td", [t._v("Operation")]), a("td", [t._v("Targets")]), a("td", [t._v("Actions")])])])
             }],
-            Ga = {
+            ei = {
                 name: "XSettings",
                 data: function() {
                     var t = "auto-flame-upgrade";
                     return {
                         successDisplayMsg: "",
                         autoUpgradeKey: t,
                         selectedAutoUpgrade: this.readAutoUpgradeFromLocalStorage(t),
-                        displayConfigs: _t(),
+                        displayConfigs: Bt(),
                         inputDisplayConfig: this.createEmptyDisplayConfigEntry(),
                         displayConfigError: "",
                         failureDisplayMsg: ""
                     }
                 },
                 computed: {
                     displayConfigsJson: function() {
-                        return Fe()(this.displayConfigs, null, 2)
+                        return Me()(this.displayConfigs, null, 2)
                     }
                 },
                 created: function() {
                     $.a.isNull(localStorage.getItem(this.autoUpgradeKey)) && this.setAutoUpgrade("relative")
                 },
                 methods: {
                     setAutoUpgrade: function(t) {
@@ -4191,37 +4325,37 @@
                                 relative_to_nodes: {
                                     type: this.inputDisplayConfig.isNameRegex ? "task_name_regex" : "task_name",
                                     value: this.inputDisplayConfig.serviceName
                                 },
                                 operation: this.inputDisplayConfig.operation,
                                 targets: this.inputDisplayConfig.targets
                             };
-                            this.displayConfigs.push(t), this.inputDisplayConfig = this.createEmptyDisplayConfigEntry(), localStorage.setItem("displayConfigs", Fe()(this.displayConfigs))
+                            this.displayConfigs.push(t), this.inputDisplayConfig = this.createEmptyDisplayConfigEntry(), localStorage.setItem("displayConfigs", Me()(this.displayConfigs))
                         }
                     },
                     deleteDisplayConfig: function(t) {
                         this.displayConfigs = $.a.filter(this.displayConfigs, function(e) {
                             return e.id !== t
-                        }), localStorage.setItem("displayConfigs", Fe()(this.displayConfigs))
+                        }), localStorage.setItem("displayConfigs", Me()(this.displayConfigs))
                     },
                     join: function(t) {
                         return $.a.join(t, ", ")
                     },
                     onCopySuccess: function() {
                         this.successDisplayMsg = "Successfully copied display config to clipboard."
                     },
                     onCopyFail: function() {
                         this.failureDisplayMsg = "Failed to copy to clipboard"
                     }
                 }
             },
-            Va = Ga,
-            Ya = (a("4d1a"), Object(Rt["a"])(Va, Ka, za, !1, null, null, null)),
-            Ja = Ya.exports,
-            Za = function() {
+            ai = ei,
+            ii = (a("4d1a"), Object(It["a"])(ai, Wa, ti, !1, null, null, null)),
+            si = ii.exports,
+            ni = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticStyle: {
                         width: "100%",
                         height: "100%",
@@ -4232,32 +4366,32 @@
                     attrs: {
                         title: t.headerParams.title,
                         links: t.headerParams.links,
                         legacyPath: t.headerParams.legacyPath
                     }
                 }), t._m(0)], 1)
             },
-            Wa = [function() {
+            ri = [function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     staticClass: "help-content"
                 }, [a("h1", [t._v("General")]), a("ul", {
                     staticClass: "shortcuts"
                 }, [a("li", [t._v("c → center the task chart")]), a("li", [t._v("r → refresh the task chart")]), a("li", [t._v("u → toggle auto update")]), a("li", [t._v("d → toggle task details in the tree view")])]), a("h1", [t._v("Searching")]), a("ul", {
                     staticClass: "shortcuts"
                 }, [a("li", [t._v("/ "), a("i", [t._v("or")]), t._v(" [CTRL] + f → enter into search mode")]), a("li", [t._v("[ENTER] → run first search/continue through results")]), a("li", [t._v("[SHIFT] + [ENTER] → reverse the search direction")]), a("li", [t._v("[ESC] → exit the search mode")])]), a("h1", [t._v("Chart Manipulation")]), a("ul", {
                     staticClass: "shortcuts"
                 }, [a("li", [t._v('[SHIFT] + [LEFT MOUSE CLICK] on task → make selected task the "root"')])])])
             }],
-            ti = {
+            oi = {
                 name: "XShortcuts",
                 components: {
-                    XHeader: sa
+                    XHeader: da
                 },
                 data: function() {
                     return {
                         headerParams: {
                             title: "Keyboard Shortcuts",
                             links: [{
                                 name: "documentation",
@@ -4277,126 +4411,126 @@
                                 icon: "question-circle"
                             }],
                             legacyPath: "/shortcuts"
                         }
                     }
                 }
             },
-            ei = ti,
-            ai = (a("7dad"), Object(Rt["a"])(ei, Za, Wa, !1, null, "173d11f4", null)),
-            ii = ai.exports;
+            ui = oi,
+            li = (a("7dad"), Object(It["a"])(ui, ni, ri, !1, null, "173d11f4", null)),
+            ci = li.exports;
         i["a"].use(w["a"]);
-        var si = new w["a"]({
+        var di = new w["a"]({
             routes: [{
                 path: "/",
-                component: $t,
+                component: Lt,
                 props: function(t) {
                     return {
                         inputLogDir: t.query.logDir,
                         inputFlameServer: t.query.flameServer
                     }
                 },
                 children: [{
                     path: "list",
                     name: "XList",
-                    component: Ba,
+                    component: Oa,
                     props: function(t) {
                         return {
                             sort: $.a.get(t.query, "sort", "alphabetical"),
                             sortDirection: $.a.get(t.query, "sortDirection", "ascending"),
                             runstates: $.a.split($.a.get(t.query, "runstates", "Completed,In-Progress"), ",")
                         }
                     }
                 }, {
                     path: "time-chart",
                     name: "XTimeChart",
-                    component: Oa,
+                    component: Ma,
                     props: function(t) {
                         return {
                             sort: $.a.get(t.query, "sort", "runtime"),
                             sortDirection: $.a.get(t.query, "sortDirection", "desc")
                         }
                     }
                 }, {
                     path: "tasks/:uuid",
                     name: "XNodeAttributes",
-                    component: Fa,
+                    component: Ka,
                     props: !0
                 }, {
                     path: "root/:rootUuid",
                     name: "custom-root",
-                    component: Aa,
+                    component: Da,
                     props: !0
                 }, {
                     path: "",
                     name: "XGraph",
-                    component: Aa,
+                    component: Da,
                     props: !0
                 }]
             }, {
                 path: "/help",
                 name: "XHelp",
-                component: Ha,
+                component: Za,
                 props: !0
             }, {
                 path: "/shortcuts",
                 name: "XShortcuts",
-                component: ii,
+                component: ci,
                 props: !0
             }, {
                 path: "/settings",
-                component: Ja
+                component: si
             }],
             scrollBehavior: function() {
                 return {
                     x: 0,
                     y: 0
                 }
             }
         });
-        si.beforeEach(function(t, e, a) {
+        di.beforeEach(function(t, e, a) {
             var i = {};
             if (e.query.logDir && !t.query.logDir && (i.logDir = e.query.logDir), e.query.flameServer && !t.query.flameServer && (i.flameServer = e.query.flameServer), $.a.isEmpty(i)) a();
             else {
                 var s = $.a.clone(t);
                 s.query = $.a.assign({}, s.query, i), a(s)
             }
         });
-        var ni = si,
-            ri = function() {
+        var pi = di,
+            fi = function() {
                 var t = this,
                     e = t.$createElement,
                     a = t._self._c || e;
                 return a("div", {
                     attrs: {
                         id: "app"
                     }
                 }, [a("router-view")], 1)
             },
-            oi = [],
-            ui = {
+            hi = [],
+            gi = {
                 name: "App"
             },
-            li = ui,
-            ci = (a("034f"), Object(Rt["a"])(li, ri, oi, !1, null, null, null)),
-            di = ci.exports,
-            pi = {
+            yi = gi,
+            mi = (a("034f"), Object(It["a"])(yi, fi, hi, !1, null, null, null)),
+            ki = mi.exports,
+            vi = {
                 allTasksByUuid: {},
                 selectedRoot: null,
                 apiConnected: !1,
                 taskNodeSizeByUuid: {},
                 search: {
                     term: "",
                     selectedIndex: 0,
                     resultUuids: [],
                     isOpen: !1
                 },
                 focusedTaskUuid: null
             },
-            fi = {
+            Ai = {
                 tasksByUuid: function(t, e) {
                     return $.a.isNull(t.selectedRoot) || !$.a.has(t.allTasksByUuid, t.selectedRoot) ? t.allTasksByUuid : e.descendantTasksByUuid(t.selectedRoot)
                 },
                 allTaskUuids: function(t, e) {
                     return $.a.keys(e.tasksByUuid)
                 },
                 runStateByUuid: function(t, e, a, i) {
@@ -4445,15 +4579,15 @@
                             return $.a.some($.a.pick(t, i), function(t) {
                                 return $.a.includes(t.toLowerCase(), a)
                             })
                         }))
                     }
                 }
             },
-            hi = {
+            Ci = {
                 setTasks: function(t, e) {
                     t.commit("setTasks", R()(e))
                 },
                 addTasksData: function(t, e) {
                     t.commit("addTasksData", e)
                 },
                 clearTaskData: function(t) {
@@ -4469,15 +4603,15 @@
                     if (e.term !== t.state.search.term) {
                         var a = t.getters.searchForUuids(e.term);
                         if (e.findUncollapsedAncestor) {
                             var i = t.rootGetters["graph/collapsedNodeUuids"],
                                 s = $.a.intersection(a, i),
                                 n = t.getters["graph/uncollapsedGraphByNodeUuid"],
                                 r = $.a.keys($.a.pickBy(n, function(t) {
-                                    return bt(t.collapsedUuids, s)
+                                    return Tt(t.collapsedUuids, s)
                                 })),
                                 o = $.a.difference(a, i),
                                 u = $.a.concat(r, o);
                             a = $.a.intersection(t.getters.allTaskUuids, u)
                         }
                         t.commit("setTaskSearchResults", {
                             term: e.term,
@@ -4493,17 +4627,17 @@
                     var e = t.state.search.resultUuids.length;
                     if (e > 0) {
                         var a = (t.state.search.selectedIndex - 1 + e) % e;
                         t.commit("setSearchIndex", a)
                     }
                 }
             },
-            gi = {
+            Ui = {
                 addTasksData: function(t, e) {
-                    t.allTasksByUuid = R()(wt(t.allTasksByUuid, e))
+                    t.allTasksByUuid = R()(Nt(t.allTasksByUuid, e))
                 },
                 setTasks: function(t, e) {
                     t.allTasksByUuid = e
                 },
                 setApiConnected: function(t, e) {
                     t.apiConnected = e
                 },
@@ -4533,86 +4667,86 @@
                 closeSearch: function(t) {
                     t.search.isOpen = !1, t.focusedTaskUuid = null
                 },
                 toggleSearchOpen: function(t) {
                     t.search.isOpen = !t.search.isOpen
                 }
             },
-            yi = {
+            xi = {
                 namespaced: !0,
-                state: pi,
-                getters: fi,
-                actions: hi,
-                mutations: gi
+                state: vi,
+                getters: Ai,
+                actions: Ci,
+                mutations: Ui
             };
 
-        function mi(t) {
+        function Si(t) {
             var e = {};
             return $.a.each(t, function(t, a) {
                 $.a.has(e, a) || (e[a] = []), $.a.isNil(t) || ($.a.has(e, t) || (e[t] = []), e[t].push(a))
             }), e
         }
 
-        function ki(t, e, a) {
+        function _i(t, e, a) {
             var i = e[t],
                 s = Object(tt["a"])({}, [t], a);
             if ($.a.isEmpty(i)) return s;
             var n = $.a.concat(t, a);
             return $.a.reduce($.a.map(i, function(t) {
-                return ki(t, e, n)
+                return _i(t, e, n)
             }), $.a.assign, s)
         }
 
-        function vi(t, e) {
-            return ki(t, e, [])
+        function Bi(t, e) {
+            return _i(t, e, [])
         }
 
-        function Ai(t, e) {
+        function Di(t, e) {
             var a = e[t];
             if ($.a.isEmpty(a)) return Object(tt["a"])({}, [t], []);
             var i = $.a.reduce($.a.map(a, function(t) {
-                return Ai(t, e)
+                return Di(t, e)
             }), $.a.assign, {});
             return i[t] = $.a.keys(i), i
         }
 
-        function Ci(t, e) {
-            return Ai(t, e)
+        function bi(t, e) {
+            return Di(t, e)
         }
 
-        function Ui(t, e, a) {
+        function Ti(t, e, a) {
             var i;
-            i = $.a.isNil(i) ? mi(e) : a;
-            var s = vi(t, i),
-                n = Ci(t, i);
+            i = $.a.isNil(i) ? Si(e) : a;
+            var s = Bi(t, i),
+                n = bi(t, i);
             return $.a.mapValues(e, function(t, a) {
                 return {
                     parentId: e[a],
                     childrenUuids: i[a],
                     ancestorUuids: s[a],
                     descendantUuids: n[a],
                     isLeaf: 0 === i[a].length
                 }
             })
         }
-        var xi = {
+        var wi = {
                 collapseConfig: {
                     uiCollapseOperationsByUuid: {},
                     hideSuccessPaths: !1,
                     applyDefaultCollapseOps: !0
                 },
                 liveUpdate: !0,
                 showTaskDetails: !1,
                 isFirstLayout: !0
             },
-            Si = {
+            Ni = {
                 graph: function(t, e, a, i) {
                     var s = $.a.mapValues(a.tasks.allTasksByUuid, "parent_id"),
-                        n = mi(s),
-                        r = Ui(i["tasks/rootUuid"], s, n);
+                        n = Si(s),
+                        r = Ti(i["tasks/rootUuid"], s, n);
                     return {
                         parentUuidByUuid: s,
                         childrenUuidsByUuid: n,
                         graphDataByUuid: r
                     }
                 },
                 parentUuidByUuid: function(t, e) {
@@ -4625,63 +4759,63 @@
                     return e.graph.graphDataByUuid
                 },
                 flameDataDisplayOperationsByUuid: function(t, e, a, i) {
                     var s = ["flame_data", "_default_display", "value"],
                         n = $.a.flatMap(i["tasks/flameDataAndNameByUuid"], function(t) {
                             return $.a.get(t, s, [])
                         });
-                    return Yt(n, i["tasks/flameDataAndNameByUuid"])
+                    return Jt(n, i["tasks/flameDataAndNameByUuid"])
                 },
                 userDisplayConfigOperationsByUuid: function(t, e) {
-                    var a = _t();
-                    return Yt(a, e.flameDataAndNameByUuid)
+                    var a = Bt();
+                    return Jt(a, e.flameDataAndNameByUuid)
                 },
                 runStateExpandOperationsByUuid: function(t, e, a, i) {
                     return ut(i["tasks/runStateByUuid"])
                 },
                 showOnlyRunStateCollapseOperationsByUuid: function(t, e, a) {
                     var i = Object(tt["a"])({}, [a.firexRunMetadata.root_uuid], [{
                         targets: ["descendants"],
                         operation: "collapse"
                     }]);
                     return $.a.assign({}, i, e.runStateExpandOperationsByUuid)
                 },
                 mergedCollapseStateSources: function(t, e) {
                     var a = [];
-                    return t.collapseConfig.applyDefaultCollapseOps && (a.push(Vt(e.flameDataDisplayOperationsByUuid, "flameData")), a.push(Vt(e.userDisplayConfigOperationsByUuid, "userConfig")), a.push(Vt(e.runStateExpandOperationsByUuid, "runState"))), t.collapseConfig.hideSuccessPaths && a.push(Vt(e.showOnlyRunStateCollapseOperationsByUuid, "runState")), a.push(t.collapseConfig.uiCollapseOperationsByUuid), $.a.mergeWith.apply($.a, [{}].concat(a, [Bt]))
+                    return t.collapseConfig.applyDefaultCollapseOps && (a.push(Yt(e.flameDataDisplayOperationsByUuid, "flameData")), a.push(Yt(e.userDisplayConfigOperationsByUuid, "userConfig")), a.push(Yt(e.runStateExpandOperationsByUuid, "runState"))), t.collapseConfig.hideSuccessPaths && a.push(Yt(e.showOnlyRunStateCollapseOperationsByUuid, "runState")), a.push(t.collapseConfig.uiCollapseOperationsByUuid), $.a.mergeWith.apply($.a, [{}].concat(a, [Dt]))
                 },
                 resolvedCollapseStateByUuid: function(t, e, a) {
                     var i = a.firexRunMetadata.root_uuid;
-                    return $.a.has(e.graphDataByUuid, i) ? ee(i, e.graphDataByUuid, e.mergedCollapseStateSources) : {}
+                    return $.a.has(e.graphDataByUuid, i) ? ae(i, e.graphDataByUuid, e.mergedCollapseStateSources) : {}
                 },
                 isCollapsedByUuid: function(t, e) {
                     return $.a.mapValues(e.resolvedCollapseStateByUuid, "collapsed")
                 },
                 collapsedNodeUuids: function(t, e) {
                     return $.a.keys($.a.pickBy(e.isCollapsedByUuid))
                 },
                 uncollapsedNodeUuids: function(t, e) {
                     return $.a.keys($.a.omitBy(e.isCollapsedByUuid))
                 },
                 uncollapsedGraphByNodeUuid: function(t, e, a, i) {
-                    var s = $.a.pick(Ut(i["tasks/rootUuid"], e.childrenUuidsByUuid, e.isCollapsedByUuid), e.uncollapsedNodeUuids);
+                    var s = $.a.pick(xt(i["tasks/rootUuid"], e.childrenUuidsByUuid, e.isCollapsedByUuid), e.uncollapsedNodeUuids);
                     return $.a.mapValues(s, function(t) {
                         return {
                             background: Ct($.a.map(t.collapsedUuids, function(t) {
                                 return i["tasks/runStateByUuid"][t].state
                             })),
                             collapsedUuids: t.collapsedUuids,
-                            widthPadding: ie * ae * 2,
-                            heightPadding: $.a.isEmpty(t.collapsedUuids) ? 0 : ie * ae,
+                            widthPadding: se * ie * 2,
+                            heightPadding: $.a.isEmpty(t.collapsedUuids) ? 0 : se * ie,
                             parent_id: t.parentId
                         }
                     })
                 }
             },
-            _i = {
+            Ei = {
                 toggleShowTaskDetails: function(t) {
                     t.commit("toggleShowTaskDetails")
                 },
                 toggleLiveUpdate: function(t) {
                     t.commit("toggleLiveUpdate")
                 },
                 setCollapseOpsByUuid: function(t, e) {
@@ -4704,15 +4838,15 @@
                     t.commit("setCollapseConfig", {
                         hideSuccessPaths: $.a.get(e, "hideSuccessPaths", !1),
                         uiCollapseOperationsByUuid: $.a.get(e, "uiCollapseOperationsByUuid", {}),
                         applyDefaultCollapseOps: $.a.get(e, "applyDefaultCollapseOps", !1)
                     })
                 }
             },
-            Bi = {
+            Oi = {
                 setCollapseOpsByUuid: function(t, e) {
                     var a = W()({}, t.collapseConfig.uiCollapseOperationsByUuid, e);
                     t.collapseConfig = W()({}, t.collapseConfig, {
                         uiCollapseOperationsByUuid: a
                     })
                 },
                 setCollapseConfig: function(t, e) {
@@ -4724,142 +4858,153 @@
                 toggleShowTaskDetails: function(t) {
                     t.showTaskDetails = !t.showTaskDetails
                 },
                 setIsFirstLayout: function(t, e) {
                     t.isFirstLayout = e
                 }
             },
-            Di = {
+            Ri = {
                 namespaced: !0,
-                state: xi,
-                getters: Si,
-                actions: _i,
-                mutations: Bi
+                state: wi,
+                getters: Ni,
+                actions: Ei,
+                mutations: Oi
             },
-            bi = {
+            Ii = {
                 uid: null,
                 logs_dir: null,
                 root_uuid: null,
                 centralServer: null,
                 flameServerUrl: null,
                 chain: null,
                 central_documentation_url: "http://firex.cisco.com"
             },
-            Ti = {
+            $i = {
                 logsUrl: function(t) {
                     var e = t.centralServer,
                         a = "";
                     return $.a.isNil(e) || (a += e), a += t.logs_dir, a
                 }
             },
-            wi = {
+            Li = {
                 setFlameRunMetadata: function(t, e) {
                     t.dispatch("tasks/clearTaskNodeSize"), t.commit("setFlameRunMetadata", e)
                 }
             },
-            Ni = {
+            Fi = {
                 setFlameRunMetadata: function(t, e) {
                     $.a.each($.a.keys(t), function(a) {
                         t[a] = e[a]
                     })
                 }
             },
-            Ei = {
+            Pi = {
                 namespaced: !0,
-                state: bi,
-                getters: Ti,
-                actions: wi,
-                mutations: Ni
+                state: Ii,
+                getters: $i,
+                actions: Li,
+                mutations: Fi
             };
-        i["a"].use(jt["a"]);
-        var Oi = !1,
-            Ri = new jt["a"].Store({
+        i["a"].use(Ht["a"]);
+        var Mi = !1,
+            Qi = new Ht["a"].Store({
                 modules: {
-                    tasks: yi,
-                    graph: Di,
-                    firexRunMetadata: Ei
+                    tasks: xi,
+                    graph: Ri,
+                    firexRunMetadata: Pi
                 },
-                strict: Oi,
-                devtools: Oi
+                strict: Mi,
+                devtools: Mi
             }),
-            Ii = !1;
-        i["a"].config.devtools = Ii, i["a"].config.performance = Ii, i["a"].use(s["a"]), i["a"].use(T.a), i["a"].config.productionTip = !1, new i["a"]({
+            Xi = !1;
+        i["a"].config.devtools = Xi, i["a"].config.performance = Xi, i["a"].use(s["a"]), i["a"].use(T.a), i["a"].config.productionTip = !1, new i["a"]({
             el: "#app",
-            router: ni,
-            store: Ri,
+            router: pi,
+            store: Qi,
             render: function(t) {
-                return t(di)
+                return t(ki)
             }
         })
     },
     "64a9": function(t, e, a) {},
-    "65cf": function(t, e, a) {
+    6604: function(t, e, a) {},
+    7071: function(t, e, a) {
         "use strict";
-        var i = a("808a"),
+        var i = a("fb85"),
             s = a.n(i);
         s.a
     },
-    6604: function(t, e, a) {},
     7441: function(t, e) {
         t.exports = "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAZAAAAGQCAYAAACAvzbMAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH4gYTFCwoTR/VAAAAAAxpVFh0Q29tbWVudAAAAAAAvK6ymQAADLxJREFUeNrt3TuqbOXWBuAxF2Kg4C3wsgMFIxGMNDHSSNAOaRO0Q5raAhtgI+xCmRQigmtVzZqXcXke+DmH/yTbmt8Y73q/uWobAQAAAAAAAABERMTiI6Czy+VyOXXAlsWMIUBAMAgaECAICeECAgRhIVRAgCAsECoIEBAYAgUBAgJDoIAAQWAgUBAgCA2ECQIEoYEwQYAgNBAmCBCEBggTBAhCA2GCAEFwIEgQIAgNhAkCBMEBgkSAIDhAkCBAhAYIEwQIggNBggBBcCBIECAIDhAkAgTBYXF5HoIEASI4LCLPz/NDgGDxTFgynrEgESBYKhaJ5+/5CxAsD8vCuXAuECAWhMXgvDgvCBCLwALAOUKA0HzoDbtz5VwJEAy4wXbenDcEiEE2xDiDCBCDa2BxJp1JAWJIDSnOqDMqQGg1mAbSmXVmESCG0BDiDCNADJ6Bw5l2pgWIITNkOOPOuACh2mAZKpx3BIhhMkg4+86+ADE8hgezYBYEiIExLJgLcyFAqDgkBgQzYkYEiKEwFJgZMyNADIIhwPyYHwHi8Dv4YJYECA48mCkzJUBGHHSHHPNlvgSIg+1gY97MmwBxmB1mMHcCxCF2gMEMmkEB4uCCWTSLAmTMgXVYwVwKEIfUIQXzKUAcTgcTzKpZFSAOJJhZMytAHEQwu2ZXgIw6gIIDzLEAcegcOjDPAsRhc9jAXJtrAZLskAkOMOMCxMFysMCsj571xYFyoMDMm3kB4iABZl+AOECAHSBAHBzALhAgDozgAHvBXmgaIA4JYD8c48mRcjjAjDK+gZz504WDCXbFtF2xOBAOBAgRO2NsgDgIgN0hQBwAwA4RIB48YJd03iV+C0t4gJk207MayFk/MThooInYK4UDxEMG7BcB4uEC9kzRPeMdiPAAzHz/BnLGTwUOEmgidk7xAPEgAbtHgHiAgBBpsIO8AwGgZwOR/IBdJEA8MECINNpJrrCEB2BH9GogRye9gwHYTw0CxMMBhEj+PTX+Ckt4AHZHkwA58+/lB9B47ghRlRDA3mrRQIQHYJcU+WefmOLCA7DDNBAAJjcQ7QPQQurtssUHDmCnrTHmCkt4AHZNowDxnQ+Aujt0RAPRPgA7Z4d/zu7JKTwAe65RA3F1BVB/p7a+wtI+ADtox38+lQ7A3tNAAOjZQLQPQAvps//aNRDhAdhNzQLEb14B9Nq1rRqI9gHYUc0aiPYB0K+FtGkg2gdgVx38z9IhCYUHoCUcvxt9DwSAfA1E+wDouyM1EAByNRDtA6D3rtRAAJgVINoH0EHlXbZLgPjiIEAee+3kkg1E+wC0kIYNRPsAmNFCyjUQ7QPQQho2EO0DYE4LKdVAtA9AC2naQAAYFHhZq5H2AUxVZZ9qIACc10C0D4B5LUQDAaBngGgfwEQVdt/DAeK7HwD1bLG7XWEB0C9AXF8Bk2XfgQ8FiOsrgLoe3eFpG4j2AZB7F3oHAsCxAeL6CqC+R3Z5ygbi+gog/050hQXAumA7uvJoHwDrZNu9GggAqwgQANa1luoVCmCSTDtYAwFgFQECQO0AcX0FUGtX3hUgvn0O0Ne9O94VFgD7NxAASBUg3n8A1NuZNweI9x8A/d2z611hAbBvA+lexQAqybA7NRAA9gsQ7z8A5rh152sgAOzXQPbi/QdA3R2qgQAgQABIFCBeoAPMc8vuP62BeP8BUHuXusICQIAAIEAAqBwgXqADzPVSBpzSQLxAB6i/U11hASBAABAgAAgQAATIBrxAB+ixW/83QPwKLwDPZYErLAC2bSAAIEAAECAACBAABMht/AovQJ8dq4EAIEAAECAAVAwQ30IH4KVM0EAA2K6BAIAAAUCAACBAABAgt/EtdIBeu1YDAUCAACBAABAgAAgQABAgAAgQAAQIAAIEAAECAAIEAAECgAABQIAAIEAAQIAAIEAAECAACBAABMjWLpfLxccN0GfXaiAACBAABAgAAgQAAQIAzwXIsiyLjwaA5zJBAwFguwYCAAIEgPoB4tvoAH12rAYCgAABQIAAIEAAECAA8FKA+DY6AM9lweENxK/yAvTYra6wABAgAAgQAAQIAB09+5tWe76U8VteANu4XC5/RsRfEfHe9T8/iIjXI+LVnrt6ueEPtkuICBCAzQLk7et/fe0aHG9ExFvXAPkqIj6LiM+v/793rv/38J4WIAD1A+TFlXsNlXcj4uOI+DAivouITyPi6+v//qYAARAgt3o9It6PiC+uLeWziPgyIj6KiFcCBECA3OPp2lQ+WZblj5QBIkQA0oXHf3f0i0ljyQNwV3jcFCAAIEAA6BEg/mZegId2qAYCQNMG4kU6wBy3rnwNBID9GsievAcBWLU7BQgAzRuI9yAA/d2z6lM0ENdYAHftzFoNBAAECADHBoj3IAB93bvi0zQQ70EAbtqVNRsIAAgQAB6y6p2Gf0shwPHO/LcPaiAAbEaAALCutTxQpVxjARwk2/WVBgLAaikDxHdCAI5pH6cEiGsmgPoeWeWusADoFSCusQDyXl89HCCusQDqenSFp77C0kIA7SMv70AAOCdAXGMB1LPF6k7fQFxjARNVWH2usABY12KqNAVXZYD2sdk+1UAAaNBAtBCAOe1DAwFgRoD4jSxA+2gaIK6YAPLaekWXu8LSQgDto2ED0UIAZrSPkg1ECwG0j6YNRAsB6N8+yjYQLQTQPpo2EAAGNJvqLcF1GaB9PLsjNRAActk1QI5oB96FABzfPjQQgJMXfOVb+EP+5N6FANy0K8u0j1YNxFUWoJEc6+mgD0U7ADioPRy1clu9A9FCACHSrIFoIQB3/0CcPnieGn7oWgjAEcWg64LXeADtQwMBEB4JHR4gRzUDV1nAJGdcurRuIEIE0D6aBYj3EwC120fECS/Rz2gIAgvo2j7OXG9PQx6MqyygXXic7dQA0QwAHtqhcwNECwG0j7qraUnyAR72CWo9QIfwyLDKUjSQI5e6JgJUl+XnYN9EByjWPtIEWbIP1FUWIDwKtI/RDcRVFkCjBnLGYtdEAO2jSQOx0AHhkT88UgZI98YDCI8uUgbI0S1EiACZZb2YSX1d5H0IML19ZF5LvgeiiQBJwyN9M7LUNREgZ3hkX0XpG8gZy1wTARLsvvR/RldYAAnbR4mQK/QwXGUBI8KjyupZij0UIQIIDwEiRADhUTU8IrwDSRtawKzwqKhcgJzVBoQIsPNuq/dn1gpqBBgcNFc/RsTPPon75n7a1VXZBqKJwK5z9UtE/OSTuGsnjAyP0gEysf2AEOkVHtU9FT/oy4kHR4ggRITH2PbRooEIERAiwkOACBEQIsJDgAgRECLCo3N4tAoQIQJCRHgIkMoHTIggRITHGE8ND/ly8kFz0hAitG8fEYW/iV5hkfvWOo3n69eI+H7S/hceAxpIpuWtjdB4vn6IiN98EnPDo3WACBEQIsJDgAgRECLCQ4AIERAiwkOACBEhAkJkbHhENP4trOxL3G9o0XS+uv521nLjXI963uO+SJhlcWsjaCKahwARIkIEhofI1AuF0dcomRa4Ky0azlen66xFeGggaZe2NoImonkIECEiRGBAiLg0GH6FlXl5u9Ki2XxVv85ahIcGUmZhayNoIpqHBqKJaCNQv4kswkMDKbmstRE0Ec1DA9FEtBEo2ETMnQbS4sBoI2giaCDaiJ+KMFtFmohZEyBtf/J3uDFTZuwMrrAaHCDXWggPNBAH309KmB9zJUAMgQMPXRqHeRIgggTMiDkSIAbEAGAuzI8AMSwGAbNgbgSI4REkOPsCRIAwZJAMBoLDnAgQQ2VAcMbNhwAxZAYFZ9pcCBADV3jgDA2TQ8MsCBBDaHgQHGZAgBhIg4Qz6twLEEMqSHAmnXcBgoE1XM6gAJnJX+d+4oHscigv/+LJelYnLHb/ZkMNxGD7yQ3nat252vvfbOgcCxDDLkyco8bnaM8QcXYFiAUgUJyX5udlrxBxVgWIxSBQnIsB52KPEHE2BYhlIVQ8/yHPf+sQESACxCIRKp7xoGe8ZYgIEAFiyVg8nt+w57dViAgQASJI2HNReR5JF/QWISJABIgggaGN8dEQESACRJDAsODYKkQEiAARJDAwOLYIEQEiQAQJDA2OR0NEgAgQYQJDQ+PREBEgAkSQCBKGB8d/5uH3iPhGgKznr3MfNtgGAefrnz/vt+GvgtdA0ErQNh6YgRevs/zgJUAQJAiOVSEiQAQIwgShsSpEBIgAQZggNFaFiAARIAgThMaqEBEgAgRhgtBYFSI+HwGCMEForAoRn5UAQaAIDFaFiM9OgCBQBAZrzu/v1y8dIkAQKAIDBAhCRViAAAGhIiwQICBchAQCBASNYAAAAAAAAAAA4Fl/A9hp9xlM0drTAAAAAElFTkSuQmCC"
     },
-    "7dad": function(t, e, a) {
+    "78a6": function(t, e, a) {
         "use strict";
-        var i = a("de4b"),
+        var i = a("02d7"),
             s = a.n(i);
         s.a
     },
-    "7f21": function(t, e, a) {},
-    "808a": function(t, e, a) {},
-    9048: function(t, e, a) {
+    "7a4d": function(t, e, a) {
         "use strict";
-        var i = a("b1ec"),
+        var i = a("9b52"),
             s = a.n(i);
         s.a
     },
-    "9b2d": function(t, e, a) {
+    "7dad": function(t, e, a) {
         "use strict";
-        var i = a("db7b"),
+        var i = a("de4b"),
             s = a.n(i);
         s.a
     },
-    ab9b: function(t, e, a) {
+    "881d": function(t, e, a) {},
+    "8d0f": function(t, e, a) {
         "use strict";
-        var i = a("ad54"),
+        var i = a("881d"),
+            s = a.n(i);
+        s.a
+    },
+    9048: function(t, e, a) {
+        "use strict";
+        var i = a("b1ec"),
             s = a.n(i);
         s.a
     },
-    ad54: function(t, e, a) {},
+    "9b52": function(t, e, a) {},
+    "9f48": function(t, e, a) {},
     afa5: function(t, e, a) {
         "use strict";
         var i = a("f8c9"),
             s = a.n(i);
         s.a
     },
     b1ec: function(t, e, a) {},
-    c3ca: function(t, e, a) {},
+    b9fa: function(t, e, a) {
+        "use strict";
+        var i = a("9f48"),
+            s = a.n(i);
+        s.a
+    },
     cfad: function(t, e, a) {},
     d005: function(t, e, a) {
         "use strict";
         var i = a("0ef1"),
             s = a.n(i);
         s.a
     },
-    db7b: function(t, e, a) {},
+    d32c: function(t, e, a) {},
     de4b: function(t, e, a) {},
-    e153: function(t, e, a) {
+    e229: function(t, e, a) {},
+    e7c1: function(t, e, a) {
         "use strict";
-        var i = a("efee"),
+        var i = a("34b2"),
             s = a.n(i);
         s.a
     },
-    e229: function(t, e, a) {},
     ee68: function(t, e, a) {
         "use strict";
         var i = a("05c2"),
             s = a.n(i);
         s.a
     },
-    efee: function(t, e, a) {},
-    f8c9: function(t, e, a) {}
+    f8c9: function(t, e, a) {},
+    fb85: function(t, e, a) {}
 });
-//# sourceMappingURL=app.19fe9253.js.map
+//# sourceMappingURL=app.d2b5e0d8.js.map
```

### Comparing `firex_flame_ui-0.4/dist/js/chunk-vendors.009e933e.js` & `firex_flame_ui-0.5/js/chunk-vendors.88295e09.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -27149,8 +27149,8 @@
             var r = n("584a").Object;
             t.exports = function(t, e) {
                 return r.getOwnPropertyDescriptor(t, e)
             }
         }
     }
 ]);
-//# sourceMappingURL=chunk-vendors.009e933e.js.map
+//# sourceMappingURL=chunk-vendors.88295e09.js.map
```

### Comparing `firex_flame_ui-0.4/dist/index.html` & `firex_flame_ui-0.5/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charset=utf-8><meta name=viewport content="width=device-width,initial-scale=1"><link href="https://fonts.googleapis.com/css?family=Source+Code+Pro|Source+Code+Pro:700|Source+Sans+Pro|Source+Sans+Pro:700" rel=stylesheet><title>Flame2</title><link href=css/app.e2e84099.css rel=preload as=style><link href=css/chunk-vendors.a2cbee8a.css rel=preload as=style><link href=js/app.19fe9253.js rel=preload as=script><link href=js/chunk-vendors.009e933e.js rel=preload as=script><link href=css/chunk-vendors.a2cbee8a.css rel=stylesheet><link href=css/app.e2e84099.css rel=stylesheet></head><body><div id=app></div><script src=js/chunk-vendors.009e933e.js></script><script src=js/app.19fe9253.js></script></body></html>
+<!DOCTYPE html><html><head><meta charset=utf-8><meta name=viewport content="width=device-width,initial-scale=1"><link href="https://fonts.googleapis.com/css?family=Source+Code+Pro|Source+Code+Pro:700|Source+Sans+Pro|Source+Sans+Pro:700" rel=stylesheet><title>Flame2</title><link href=css/app.2e01ad42.css rel=preload as=style><link href=css/chunk-vendors.a2cbee8a.css rel=preload as=style><link href=js/app.d2b5e0d8.js rel=preload as=script><link href=js/chunk-vendors.88295e09.js rel=preload as=script><link href=css/chunk-vendors.a2cbee8a.css rel=stylesheet><link href=css/app.2e01ad42.css rel=stylesheet></head><body><div id=app></div><script src=js/chunk-vendors.88295e09.js></script><script src=js/app.d2b5e0d8.js></script></body></html>
```

### Comparing `firex_flame_ui-0.4/setup.py` & `firex_flame_ui-0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from setuptools import setup
 # import versioneer
 
 setup(name='firex_flame_ui',
       # version=versioneer.get_version(),
-      version='0.4',
+      version='0.5',
       # cmdclass=versioneer.get_cmdclass(),
       description='UI for FireX.',
       url='https://github.com/FireXStuff/firex-flame-ui',
       author='Core FireX Team',
       author_email='firex-dev@gmail.com',
       license='BSD-3-Clause',
       packages=['firex_flame_ui'],
-      # npm run build puts artifact in the 'dist' directory.
-      package_dir={'firex_flame_ui': 'dist'},
+      # 'npm run build' is configured to put build artifacts & files in this 'public' folder in the 'dist' directory.
+      # Therefore, at python packaging time, both python files & UI build artifacts are in the same (current) directory.
+      package_dir={'firex_flame_ui': './'},
       zip_safe=True,
       include_package_data=True,
       package_data={
-        'firex_flame_ui': ['*.html', 'js/*.js', 'img/*', 'css/*.css'],
+            # Files available to consumers of this python package (UI build artifacts).
+            # NOTE: these expressions must also be present in MANIFEST.in
+            'firex_flame_ui': ['*.html', 'js/*.js', 'img/*', 'css/*.css', 'COMMITHASH'],
       },
       entry_points={},
       )
 
-
```

