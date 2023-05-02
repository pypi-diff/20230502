# Comparing `tmp/mkdocs-1.4.1.tar.gz` & `tmp/mkdocs-1.4.2.tar.gz`

## Comparing `mkdocs-1.4.1.tar` & `mkdocs-1.4.2.tar`

### file list

```diff
@@ -1,223 +1,227 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/__init__.py
--rw-r--r--   0        0        0    10045 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/__main__.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/exceptions.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/localization.py
--rw-r--r--   0        0        0    17936 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/py.typed
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/theme.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/commands/__init__.py
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/commands/babel.py
--rw-r--r--   0        0        0    12419 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/commands/build.py
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/commands/gh_deploy.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/commands/new.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/commands/serve.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/commands/setup.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/config/__init__.py
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/config/base.py
--rw-r--r--   0        0        0    36992 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/config/config_options.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/config/defaults.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/__init__.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/__init__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/prebuild-index.js
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/search_index.py
--rw-r--r--   0        0        0    24525 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.ar.js
--rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.da.js
--rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.de.js
--rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.du.js
--rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.es.js
--rw-r--r--   0        0        0    20949 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.fi.js
--rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.fr.js
--rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.hu.js
--rw-r--r--   0        0        0    24077 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.it.js
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.ja.js
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.jp.js
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.multi.js
--rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.nl.js
--rw-r--r--   0        0        0     9947 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.no.js
--rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.pt.js
--rw-r--r--   0        0        0    23151 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.ro.js
--rw-r--r--   0        0        0    19108 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.ru.js
--rw-r--r--   0        0        0    13504 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.sv.js
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.th.js
--rw-r--r--   0        0        0    38283 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.tr.js
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.vi.js
--rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/tinyseg.js
--rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/templates/search/lunr.js
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/templates/search/main.js
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/contrib/search/templates/search/worker.js
--rw-r--r--   0        0        0    12169 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/livereload/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/structure/__init__.py
--rw-r--r--   0        0        0    12689 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/structure/files.py
--rw-r--r--   0        0        0     8411 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/structure/nav.py
--rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/structure/pages.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/structure/toc.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/templates/sitemap.xml
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/__init__.py
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/base.py
--rw-r--r--   0        0        0    24365 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/build_tests.py
--rw-r--r--   0        0        0    24797 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/cli_tests.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/gh_deploy_tests.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration.py
--rw-r--r--   0        0        0    24185 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/livereload_tests.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/localization_tests.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/new_tests.py
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/plugin_tests.py
--rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/search_tests.py
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/theme_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/config/__init__.py
--rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/config/base_tests.py
--rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/config/config_options_legacy_tests.py
--rw-r--r--   0        0        0    70040 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/config/config_options_tests.py
--rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/config/config_tests.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/complicated_config/mkdocs.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/complicated_config/documentation/custom.html
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/complicated_config/documentation/index.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/complicated_config/documentation/tweak.css
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/complicated_config/documentation/tweak.js
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/complicated_config/theme_tweaks/404.html
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/minimal/mkdocs.yml
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/minimal/docs/testing.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/mkdocs.yml
--rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/image.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/index.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/metadata.md
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/non-index.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/page-title.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/pageTitle.md
--rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/sub1/image.png
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/sub1/index.md
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/sub1/non-index.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/sub1/sub1a/index.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/sub1/sub1a/non-index.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/sub2/index.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/sub2/non-index.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/unicode/mkdocs.yml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/unicode/docs/index.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/unicode/docs/Übersicht.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/integration/unicode/docs/♪.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/structure/__init__.py
--rw-r--r--   0        0        0    34572 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/structure/file_tests.py
--rw-r--r--   0        0        0    19542 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/structure/nav_tests.py
--rw-r--r--   0        0        0    35314 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/structure/page_tests.py
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/structure/toc_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/utils/__init__.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/utils/babel_stub_tests.py
--rw-r--r--   0        0        0    24090 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/tests/utils/utils_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/babel.cfg
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/404.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/__init__.py
--rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/base.html
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/content.html
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/keyboard-modal.html
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/main.html
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/messages.pot
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/mkdocs_theme.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/nav-sub.html
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/search-modal.html
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/toc.html
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/css/base.css
--rw-r--r--   0        0        0   163091 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/css/font-awesome.min.css
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/img/favicon.ico
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/img/grid.png
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/js/base.js
--rw-r--r--   0        0        0    58073 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/js/bootstrap.min.js
--rw-r--r--   0        0        0    93107 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/js/jquery-1.10.2.min.js
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/tr_TR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/tr_TR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/404.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/base.html
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/breadcrumbs.html
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/footer.html
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/main.html
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/messages.pot
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/mkdocs_theme.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/nav.html
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/search.html
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/searchbox.html
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/toc.html
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/versions.html
--rw-r--r--   0        0        0   129978 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/theme.css
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/theme_extra.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/img/favicon.ico
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/js/html5shiv.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/js/theme.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/js/theme_extra.js
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/tr_TR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/tr_TR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    13642 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/utils/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/utils/babel_stub.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/utils/filters.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 mkdocs-1.4.1/mkdocs/utils/meta.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs-1.4.1/.gitignore
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs-1.4.1/LICENSE
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 mkdocs-1.4.1/README.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mkdocs-1.4.1/hatch_build.py
--rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 mkdocs-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 mkdocs-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/__init__.py
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/__main__.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/exceptions.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/localization.py
+-rw-r--r--   0        0        0    18066 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/py.typed
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/theme.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/commands/__init__.py
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/commands/babel.py
+-rw-r--r--   0        0        0    12419 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/commands/build.py
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/commands/gh_deploy.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/commands/new.py
+-rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/commands/serve.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/commands/setup.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/config/__init__.py
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/config/base.py
+-rw-r--r--   0        0        0    37863 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/config/config_options.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/config/defaults.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/__init__.py
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/__init__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/prebuild-index.js
+-rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/search_index.py
+-rw-r--r--   0        0        0    24525 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.ar.js
+-rw-r--r--   0        0        0    10349 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.da.js
+-rw-r--r--   0        0        0    13949 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.de.js
+-rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.du.js
+-rw-r--r--   0        0        0    24406 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.es.js
+-rw-r--r--   0        0        0    20949 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.fi.js
+-rw-r--r--   0        0        0    25654 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.fr.js
+-rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.hu.js
+-rw-r--r--   0        0        0    24077 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.it.js
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.ja.js
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.jp.js
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.multi.js
+-rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.nl.js
+-rw-r--r--   0        0        0     9947 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.no.js
+-rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.pt.js
+-rw-r--r--   0        0        0    23151 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.ro.js
+-rw-r--r--   0        0        0    19108 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.ru.js
+-rw-r--r--   0        0        0    13504 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.sv.js
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.th.js
+-rw-r--r--   0        0        0    38283 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.tr.js
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.vi.js
+-rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/tinyseg.js
+-rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/templates/search/lunr.js
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/templates/search/main.js
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/contrib/search/templates/search/worker.js
+-rw-r--r--   0        0        0    12427 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/livereload/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/structure/__init__.py
+-rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/structure/files.py
+-rw-r--r--   0        0        0     8411 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/structure/nav.py
+-rw-r--r--   0        0        0    12516 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/structure/pages.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/structure/toc.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/templates/sitemap.xml
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/__init__.py
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/base.py
+-rw-r--r--   0        0        0    24365 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/build_tests.py
+-rw-r--r--   0        0        0    24797 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/cli_tests.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/gh_deploy_tests.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration.py
+-rw-r--r--   0        0        0    24185 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/livereload_tests.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/localization_tests.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/new_tests.py
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/plugin_tests.py
+-rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/search_tests.py
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/theme_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/config/__init__.py
+-rw-r--r--   0        0        0    10661 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/config/base_tests.py
+-rw-r--r--   0        0        0    54779 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/config/config_options_legacy_tests.py
+-rw-r--r--   0        0        0    71711 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/config/config_options_tests.py
+-rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/config/config_tests.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/complicated_config/mkdocs.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/complicated_config/documentation/custom.html
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/complicated_config/documentation/index.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/complicated_config/documentation/tweak.css
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/complicated_config/documentation/tweak.js
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/complicated_config/theme_tweaks/404.html
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/minimal/mkdocs.yml
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/minimal/docs/testing.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/mkdocs.yml
+-rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/image.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/index.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/metadata.md
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/non-index.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/page-title.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/pageTitle.md
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/sub1/image.png
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/sub1/index.md
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/sub1/non-index.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/sub1/sub1a/index.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/sub1/sub1a/non-index.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/sub2/index.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/sub2/non-index.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/unicode/mkdocs.yml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/unicode/docs/index.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/unicode/docs/Übersicht.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/integration/unicode/docs/♪.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/structure/__init__.py
+-rw-r--r--   0        0        0    34583 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/structure/file_tests.py
+-rw-r--r--   0        0        0    19542 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/structure/nav_tests.py
+-rw-r--r--   0        0        0    35316 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/structure/page_tests.py
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/structure/toc_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/utils/babel_stub_tests.py
+-rw-r--r--   0        0        0    24084 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/tests/utils/utils_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/babel.cfg
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/404.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/__init__.py
+-rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/base.html
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/content.html
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/keyboard-modal.html
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/main.html
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/messages.pot
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/mkdocs_theme.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/nav-sub.html
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/search-modal.html
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/toc.html
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/css/base.css
+-rw-r--r--   0        0        0   163091 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/css/bootstrap.min.css
+-rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/css/font-awesome.min.css
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/img/favicon.ico
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/img/grid.png
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/js/base.js
+-rw-r--r--   0        0        0    58073 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/js/bootstrap.min.js
+-rw-r--r--   0        0        0    93107 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/js/jquery-1.10.2.min.js
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/nb/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/nn/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/tr_TR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/tr_TR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/404.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/base.html
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/breadcrumbs.html
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/footer.html
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/main.html
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/messages.pot
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/mkdocs_theme.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/nav.html
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/search.html
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/searchbox.html
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/toc.html
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/versions.html
+-rw-r--r--   0        0        0   129978 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/theme.css
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/theme_extra.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/img/favicon.ico
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/js/html5shiv.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/js/theme.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/js/theme_extra.js
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/tr_TR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/tr_TR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    13718 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/utils/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/utils/babel_stub.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/utils/filters.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 mkdocs-1.4.2/mkdocs/utils/meta.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs-1.4.2/LICENSE
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 mkdocs-1.4.2/README.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mkdocs-1.4.2/hatch_build.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 mkdocs-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 mkdocs-1.4.2/PKG-INFO
```

### Comparing `mkdocs-1.4.1/mkdocs/__main__.py` & `mkdocs-1.4.2/mkdocs/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 pass_state = click.make_pass_decorator(State, ensure=True)
 
 clean_help = "Remove old files from the site_dir before building (the default)."
 config_help = "Provide a specific MkDocs config"
 dev_addr_help = "IP address and port to serve documentation locally (default: localhost:8000)"
 strict_help = "Enable strict mode. This will cause MkDocs to abort the build on any warnings."
 theme_help = "The theme to use when building your documentation."
-theme_choices = utils.get_theme_names()
+theme_choices = sorted(utils.get_theme_names())
 site_dir_help = "The directory to output the result of the documentation build."
 use_directory_urls_help = "Use directory URLs when building pages (the default)."
 reload_help = "Enable the live reloading in the development server (this is the default)"
 no_reload_help = "Disable the live reloading in the development server."
 dirty_reload_help = (
     "Enable the live reloading in the development server, but only re-build files that have changed"
 )
```

### Comparing `mkdocs-1.4.1/mkdocs/exceptions.py` & `mkdocs-1.4.2/mkdocs/exceptions.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/localization.py` & `mkdocs-1.4.2/mkdocs/localization.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         # no babel installed, add dummy support for trans/endtrans blocks
         env.add_extension(NoBabelExtension)
         env.install_null_translations()
 
 
 def _get_merged_translations(
     theme_dirs: Sequence[str], locales_dir: str, locale: Locale
-) -> Translations:
+) -> Optional[Translations]:
     merged_translations: Optional[Translations] = None
 
     log.debug(f"Looking for translations for locale '{locale}'")
     if locale.territory:
         locale_str = f"{locale.language}_{locale.territory}"
     else:
         locale_str = locale.language
```

### Comparing `mkdocs-1.4.1/mkdocs/plugins.py` & `mkdocs-1.4.2/mkdocs/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     All plugins should subclass this class.
     """
 
     config_class: Type[SomeConfig] = LegacyConfig  # type: ignore[assignment]
     config_scheme: PlainConfigSchema = ()
     config: SomeConfig = {}  # type: ignore[assignment]
 
+    supports_multiple_instances: bool = False
+    """Set to true in subclasses to declare support for adding the same plugin multiple times."""
+
     def __class_getitem__(cls, config_class: Type[Config]):
         """Eliminates the need to write `config_class = FooConfig` when subclassing BasePlugin[FooConfig]"""
         name = f'{cls.__name__}[{config_class.__name__}]'
         return type(name, (cls,), dict(config_class=config_class))
 
     def __init_subclass__(cls):
         if not issubclass(cls.config_class, Config):
@@ -495,15 +498,15 @@
     def run_event(self, name: str, item: None = None, **kwargs) -> Any:
         ...
 
     @overload
     def run_event(self, name: str, item: T, **kwargs) -> T:
         ...
 
-    def run_event(self, name: str, item=None, **kwargs) -> Optional[T]:
+    def run_event(self, name: str, item=None, **kwargs):
         """
         Run all registered methods of an event.
 
         `item` is the object to be modified or replaced and returned by the event method.
         If it isn't given the event method creates a new object to be returned.
         All other keywords are variables for context, but would not generally
         be modified by the event method.
```

### Comparing `mkdocs-1.4.1/mkdocs/theme.py` & `mkdocs-1.4.2/mkdocs/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/commands/babel.py` & `mkdocs-1.4.2/mkdocs/commands/babel.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/commands/build.py` & `mkdocs-1.4.2/mkdocs/commands/build.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/commands/gh_deploy.py` & `mkdocs-1.4.2/mkdocs/commands/gh_deploy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 from __future__ import annotations
 
 import logging
 import os
 import re
 import subprocess
+from typing import Optional, Tuple, Union
 
 import ghp_import
 from packaging import version
 
 import mkdocs
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.exceptions import Abort
 
 log = logging.getLogger(__name__)
 
 default_message = """Deployed {sha} with MkDocs version: {version}"""
 
 
-def _is_cwd_git_repo():
+def _is_cwd_git_repo() -> bool:
     try:
         proc = subprocess.Popen(
             ['git', 'rev-parse', '--is-inside-work-tree'],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
     except FileNotFoundError:
         log.error("Could not find git - is it installed and on your path?")
         raise Abort('Deployment Aborted!')
     proc.communicate()
     return proc.wait() == 0
 
 
-def _get_current_sha(repo_path):
+def _get_current_sha(repo_path) -> str:
     proc = subprocess.Popen(
         ['git', 'rev-parse', '--short', 'HEAD'],
         cwd=repo_path or None,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
 
     stdout, _ = proc.communicate()
     sha = stdout.decode('utf-8').strip()
     return sha
 
 
-def _get_remote_url(remote_name):
+def _get_remote_url(remote_name: str) -> Union[Tuple[str, str], Tuple[None, None]]:
     # No CNAME found.  We will use the origin URL to determine the GitHub
     # pages location.
     remote = f"remote.{remote_name}.url"
     proc = subprocess.Popen(
         ["git", "config", "--get", remote],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
 
     stdout, _ = proc.communicate()
     url = stdout.decode('utf-8').strip()
 
-    host = None
-    path = None
     if 'github.com/' in url:
         host, path = url.split('github.com/', 1)
     elif 'github.com:' in url:
         host, path = url.split('github.com:', 1)
-
+    else:
+        return None, None
     return host, path
 
 
-def _check_version(branch):
+def _check_version(branch: str) -> None:
     proc = subprocess.Popen(
         ['git', 'show', '-s', '--format=%s', f'refs/heads/{branch}'],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
 
     stdout, _ = proc.communicate()
@@ -93,20 +93,20 @@
             'to deploy anyway.'
         )
         raise Abort('Deployment Aborted!')
 
 
 def gh_deploy(
     config: MkDocsConfig,
-    message=None,
+    message: Optional[str] = None,
     force=False,
     no_history=False,
     ignore_version=False,
     shell=False,
-):
+) -> None:
     if not _is_cwd_git_repo():
         log.error('Cannot deploy - this directory does not appear to be a git repository')
 
     remote_branch = config.remote_branch
     remote_name = config.remote_name
 
     if not ignore_version:
@@ -152,15 +152,15 @@
         log.info(
             'NOTE: Your DNS records must be configured appropriately for your CNAME URL to work.'
         )
         return
 
     host, path = _get_remote_url(remote_name)
 
-    if host is None:
+    if host is None or path is None:
         # This could be a GitHub Enterprise deployment.
         log.info('Your documentation should be available shortly.')
     else:
         username, repo = path.split('/', 1)
         if repo.endswith('.git'):
             repo = repo[: -len('.git')]
         url = f'https://{username}.github.io/{repo}/'
```

### Comparing `mkdocs-1.4.1/mkdocs/commands/new.py` & `mkdocs-1.4.2/mkdocs/commands/new.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/commands/serve.py` & `mkdocs-1.4.2/mkdocs/commands/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import functools
 import logging
 import shutil
 import tempfile
 from os.path import isdir, isfile, join
+from typing import Optional
 from urllib.parse import urlsplit
 
 import jinja2.exceptions
 
 from mkdocs.commands.build import build
 from mkdocs.config import load_config
 from mkdocs.config.defaults import MkDocsConfig
@@ -54,15 +55,15 @@
         site_dir=site_dir,
         **kwargs,
     )
 
     live_server = livereload in ('dirty', 'livereload')
     dirty = livereload == 'dirty'
 
-    def builder(config=None):
+    def builder(config: Optional[MkDocsConfig] = None):
         log.info("Building documentation...")
         if config is None:
             config = get_config()
 
         # combine CLI watch arguments with config file values
         if config.watch is None:
             config.watch = watch
@@ -82,20 +83,21 @@
         builder(config)
 
         host, port = config.dev_addr
         server = LiveReloadServer(
             builder=builder, host=host, port=port, root=site_dir, mount_path=mount_path(config)
         )
 
-        def error_handler(code):
+        def error_handler(code) -> Optional[bytes]:
             if code in (404, 500):
                 error_page = join(site_dir, f'{code}.html')
                 if isfile(error_page):
                     with open(error_page, 'rb') as f:
                         return f.read()
+            return None
 
         server.error_handler = error_handler
 
         if live_server:
             # Watch the documentation files, the config file and the theme files.
             server.watch(config.docs_dir)
             server.watch(config.config_file_path)
```

### Comparing `mkdocs-1.4.1/mkdocs/commands/setup.py` & `mkdocs-1.4.2/mkdocs/commands/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/config/base.py` & `mkdocs-1.4.2/mkdocs/config/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,21 +359,21 @@
 
     # Then load the options to overwrite anything in the config.
     cfg.load_dict(options)
 
     errors, warnings = cfg.validate()
 
     for config_name, warning in warnings:
-        log.warning(f"Config value: '{config_name}'. Warning: {warning}")
+        log.warning(f"Config value '{config_name}': {warning}")
 
     for config_name, error in errors:
-        log.error(f"Config value: '{config_name}'. Error: {error}")
+        log.error(f"Config value '{config_name}': {error}")
 
     for key, value in cfg.items():
-        log.debug(f"Config value: '{key}' = {value!r}")
+        log.debug(f"Config value '{key}' = {value!r}")
 
     if len(errors) > 0:
         raise exceptions.Abort(f"Aborted with {len(errors)} Configuration Errors!")
     elif cfg['strict'] and len(warnings) > 0:
         raise exceptions.Abort(
             f"Aborted with {len(warnings)} Configuration Warnings in 'strict' mode!"
         )
```

### Comparing `mkdocs-1.4.1/mkdocs/config/config_options.py` & `mkdocs-1.4.2/mkdocs/config/config_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 import os
 import string
 import sys
 import traceback
 import types
 import typing as t
 import warnings
-from collections import UserString
+from collections import Counter, UserString
 from typing import (
     Any,
     Collection,
     Dict,
     Generic,
     Iterator,
     List,
     Mapping,
+    MutableMapping,
     NamedTuple,
     Tuple,
     TypeVar,
     Union,
     overload,
 )
 from urllib.parse import quote as urlquote
@@ -92,19 +93,19 @@
             config.load_dict(value)
             failed, warnings = config.validate()
         except ConfigurationError as e:
             raise ValidationError(str(e))
 
         if self._do_validation:
             # Capture errors and warnings
-            self.warnings = [f'Sub-option {key!r}: {msg}' for key, msg in warnings]
+            self.warnings = [f"Sub-option '{key}': {msg}" for key, msg in warnings]
             if failed:
                 # Get the first failing one
                 key, err = failed[0]
-                raise ValidationError(f"Sub-option {key!r} configuration error: {err}")
+                raise ValidationError(f"Sub-option '{key}': {err}")
 
         return config
 
 
 class OptionallyRequired(Generic[T], BaseConfigOption[T]):
     """
     Soft-deprecated, do not use.
@@ -305,15 +306,15 @@
         self.moved_to = moved_to
         if not message:
             if removed:
                 message = "The configuration option '{}' was removed from MkDocs."
             else:
                 message = (
                     "The configuration option '{}' has been deprecated and "
-                    "will be removed in a future release of MkDocs."
+                    "will be removed in a future release."
                 )
             if moved_to:
                 message += f" Use '{moved_to}' instead."
 
         self.message = message
         self.removed = removed
         self.option = option_type or BaseConfigOption()
@@ -929,17 +930,17 @@
     def pre_validation(self, config, key_name):
         self._config = config
 
     def run_validation(self, value: object) -> plugins.PluginCollection:
         if not isinstance(value, (list, tuple, dict)):
             raise ValidationError('Invalid Plugins configuration. Expected a list or dict.')
         self.plugins = plugins.PluginCollection()
+        self._instance_counter: MutableMapping[str, int] = Counter()
         for name, cfg in self._parse_configs(value):
-            name, plugin = self.load_plugin_with_namespace(name, cfg)
-            self.plugins[name] = plugin
+            self.load_plugin_with_namespace(name, cfg)
         return self.plugins
 
     @classmethod
     def _parse_configs(cls, value: Union[list, tuple, dict]) -> Iterator[Tuple[str, dict]]:
         if isinstance(value, dict):
             for name, cfg in value.items():
                 if not isinstance(name, str):
@@ -977,36 +978,55 @@
         if name not in self.installed_plugins:
             raise ValidationError(f'The "{name}" plugin is not installed')
 
         config = config or {}  # Users may define a null (None) config
         if not isinstance(config, dict):
             raise ValidationError(f"Invalid config options for the '{name}' plugin.")
 
-        plugin = self.plugin_cache.get(name)
+        self._instance_counter[name] += 1
+        inst_number = self._instance_counter[name]
+        inst_name = name
+        if inst_number > 1:
+            inst_name += f' #{inst_number}'
+
+        plugin = self.plugin_cache.get(inst_name)
         if plugin is None:
             plugin_cls = self.installed_plugins[name].load()
 
             if not issubclass(plugin_cls, plugins.BasePlugin):
                 raise ValidationError(
                     f'{plugin_cls.__module__}.{plugin_cls.__name__} must be a subclass of'
                     f' {plugins.BasePlugin.__module__}.{plugins.BasePlugin.__name__}'
                 )
 
             plugin = plugin_cls()
 
             if hasattr(plugin, 'on_startup') or hasattr(plugin, 'on_shutdown'):
-                self.plugin_cache[name] = plugin
+                self.plugin_cache[inst_name] = plugin
+
+        if inst_number > 1 and not getattr(plugin, 'supports_multiple_instances', False):
+            self.warnings.append(
+                f"Plugin '{name}' was specified multiple times - this is likely a mistake, "
+                "because the plugin doesn't declare `supports_multiple_instances`."
+            )
 
-        errors, warnings = plugin.load_config(
+        errors, warns = plugin.load_config(
             config, self._config.config_file_path if self._config else None
         )
-        self.warnings.extend(f"Plugin '{name}' value: '{x}'. Warning: {y}" for x, y in warnings)
-        errors_message = '\n'.join(f"Plugin '{name}' value: '{x}'. Error: {y}" for x, y in errors)
+        for warning in warns:
+            if isinstance(warning, str):
+                self.warnings.append(f"Plugin '{inst_name}': {warning}")
+            else:
+                key, msg = warning
+                self.warnings.append(f"Plugin '{inst_name}' option '{key}': {msg}")
+
+        errors_message = '\n'.join(f"Plugin '{name}' option '{key}': {msg}" for key, msg in errors)
         if errors_message:
             raise ValidationError(errors_message)
+        self.plugins[inst_name] = plugin
         return plugin
 
 
 class Hooks(BaseConfigOption[List[types.ModuleType]]):
     """A list of Python scripts to be treated as instances of plugins."""
 
     def __init__(self, plugins_key: str) -> None:
@@ -1032,14 +1052,16 @@
     def _load_hook(self, name, path):
         import importlib.util
 
         spec = importlib.util.spec_from_file_location(name, path)
         if spec is None:
             raise ValidationError(f"Cannot import path '{path}' as a Python module")
         module = importlib.util.module_from_spec(spec)
+        if spec.loader is None:
+            raise ValidationError(f"Cannot import path '{path}' as a Python module")
         spec.loader.exec_module(module)
         return module
 
     def post_validation(self, config: Config, key_name: str):
         plugins = config[self.plugins_key]
         for name, hook in config[key_name].items():
             plugins[name] = hook
```

### Comparing `mkdocs-1.4.1/mkdocs/config/defaults.py` & `mkdocs-1.4.2/mkdocs/config/defaults.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/__init__.py` & `mkdocs-1.4.2/mkdocs/contrib/search/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
         fallback = {'uk': 'ru'}
         for lang_part in lang.split("_"):
             lang_part = lang_part.lower()
             lang_part = fallback.get(lang_part, lang_part)
             if os.path.isfile(os.path.join(base_path, 'lunr-language', f'lunr.{lang_part}.js')):
                 return lang_part
 
-    def run_validation(self, value):
+    def run_validation(self, value: object):
         if isinstance(value, str):
             value = [value]
-        elif not isinstance(value, (list, tuple)):
+        if not isinstance(value, list):
             raise c.ValidationError('Expected a list of language codes.')
         for lang in list(value):
             if lang != 'en':
                 lang_detected = self.get_lunr_supported_lang(lang)
                 if not lang_detected:
                     log.info(f"Option search.lang '{lang}' is not supported, falling back to 'en'")
                     value.remove(lang)
```

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/prebuild-index.js` & `mkdocs-1.4.2/mkdocs/contrib/search/prebuild-index.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/search_index.py` & `mkdocs-1.4.2/mkdocs/contrib/search/search_index.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.ar.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.ar.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.da.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.da.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.de.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.de.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.du.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.du.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.es.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.es.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.fi.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.fi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.fr.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.fr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.hu.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.hu.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.it.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.it.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.ja.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.ja.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.multi.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.multi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.nl.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.nl.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.no.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.no.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.pt.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.pt.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.ro.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.ro.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.ru.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.ru.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.stemmer.support.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.sv.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.sv.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.th.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.th.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.tr.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.tr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/lunr.vi.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/lunr.vi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/lunr-language/tinyseg.js` & `mkdocs-1.4.2/mkdocs/contrib/search/lunr-language/tinyseg.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/templates/search/lunr.js` & `mkdocs-1.4.2/mkdocs/contrib/search/templates/search/lunr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/templates/search/main.js` & `mkdocs-1.4.2/mkdocs/contrib/search/templates/search/main.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/contrib/search/templates/search/worker.js` & `mkdocs-1.4.2/mkdocs/contrib/search/templates/search/worker.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/livereload/__init__.py` & `mkdocs-1.4.2/mkdocs/livereload/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 import socketserver
 import string
 import threading
 import time
 import urllib.parse
 import warnings
 import wsgiref.simple_server
-from typing import Any, Callable, Dict, Optional, Tuple
+import wsgiref.util
+from typing import Any, BinaryIO, Callable, Dict, Iterable, Optional, Tuple
 
 import watchdog.events
 import watchdog.observers.polling
 
 _SCRIPT_TEMPLATE_STR = """
 var livereload = function(epoch, requestId) {
     var req = new XMLHttpRequest();
@@ -58,15 +59,15 @@
 
 class LiveReloadServer(socketserver.ThreadingMixIn, wsgiref.simple_server.WSGIServer):
     daemon_threads = True
     poll_response_timeout = 60
 
     def __init__(
         self,
-        builder: Callable,
+        builder: Callable[[], None],
         host: str,
         port: int,
         root: str,
         mount_path: str = "/",
         polling_interval: float = 0.5,
         shutdown_delay: float = 0.25,
         **kwargs,
@@ -81,39 +82,44 @@
             pass
         self.root = os.path.abspath(root)
         self.mount_path = ("/" + mount_path.lstrip("/")).rstrip("/") + "/"
         self.url = f"http://{self.server_name}:{self.server_port}{self.mount_path}"
         self.build_delay = 0.1
         self.shutdown_delay = shutdown_delay
         # To allow custom error pages.
-        self.error_handler = lambda code: None
+        self.error_handler: Callable[[int], Optional[bytes]] = lambda code: None
 
         super().__init__((host, port), _Handler, **kwargs)
         self.set_app(self.serve_request)
 
         self._wanted_epoch = _timestamp()  # The version of the site that started building.
         self._visible_epoch = self._wanted_epoch  # Latest fully built version of the site.
         self._epoch_cond = threading.Condition()  # Must be held when accessing _visible_epoch.
 
-        self._to_rebuild: Dict[Callable, bool] = {}  # Used as an ordered set of functions to call.
+        self._to_rebuild: Dict[
+            Callable[[], None], bool
+        ] = {}  # Used as an ordered set of functions to call.
         self._rebuild_cond = threading.Condition()  # Must be held when accessing _to_rebuild.
 
         self._shutdown = False
         self.serve_thread = threading.Thread(target=lambda: self.serve_forever(shutdown_delay))
         self.observer = watchdog.observers.polling.PollingObserver(timeout=polling_interval)
 
         self._watched_paths: Dict[str, int] = {}
         self._watch_refs: Dict[str, Any] = {}
 
-    def watch(self, path: str, func: Optional[Callable] = None, recursive: bool = True) -> None:
+    def watch(
+        self, path: str, func: Optional[Callable[[], None]] = None, recursive: bool = True
+    ) -> None:
         """Add the 'path' to watched paths, call the function and reload when any file changes under it."""
         path = os.path.abspath(path)
-        if func in (None, self.builder):
-            func = self.builder
+        if func is None or func is self.builder:
+            funct = self.builder
         else:
+            funct = func
             warnings.warn(
                 "Plugins should not pass the 'func' parameter of watch(). "
                 "The ability to execute custom callbacks will be removed soon.",
                 DeprecationWarning,
                 stacklevel=2,
             )
 
@@ -123,15 +129,15 @@
         self._watched_paths[path] = 1
 
         def callback(event):
             if event.is_directory:
                 return
             log.debug(str(event))
             with self._rebuild_cond:
-                self._to_rebuild[func] = True
+                self._to_rebuild[funct] = True
                 self._rebuild_cond.notify_all()
 
         handler = watchdog.events.FileSystemEventHandler()
         handler.on_any_event = callback
         log.debug(f"Watching '{path}'")
         self._watch_refs[path] = self.observer.schedule(handler, path, recursive=recursive)
 
@@ -190,15 +196,15 @@
 
         if self.serve_thread.is_alive():
             super().shutdown()
         if wait:
             self.serve_thread.join()
             self.observer.join()
 
-    def serve_request(self, environ, start_response):
+    def serve_request(self, environ, start_response) -> Iterable[bytes]:
         try:
             result = self._serve_request(environ, start_response)
         except Exception:
             code = 500
             msg = "500 Internal Server Error"
             log.exception(msg)
         else:
@@ -214,15 +220,15 @@
             log.exception("Failed to render an error message!")
         if error_content is None:
             error_content = msg.encode()
 
         start_response(msg, [("Content-Type", "text/html")])
         return [error_content]
 
-    def _serve_request(self, environ, start_response):
+    def _serve_request(self, environ, start_response) -> Optional[Iterable[bytes]]:
         # https://bugs.python.org/issue16679
         # https://github.com/bottlepy/bottle/blob/f9b1849db4/bottle.py#L984
         path = environ["PATH_INFO"].encode("latin-1").decode("utf-8", "ignore")
 
         if path.startswith("/livereload/"):
             m = re.fullmatch(r"/livereload/([0-9]+)/[0-9]+", path)
             if m:
@@ -236,15 +242,15 @@
                     if not condition():
                         # Stall the browser, respond as soon as there's something new.
                         # If there's not, respond anyway after a minute.
                         self._log_poll_request(environ.get("HTTP_REFERER"), request_id=path)
                         self._epoch_cond.wait_for(condition, timeout=self.poll_response_timeout)
                     return [b"%d" % self._visible_epoch]
 
-        if path.startswith(self.mount_path):
+        if (path + "/").startswith(self.mount_path):
             rel_file_path = path[len(self.mount_path) :]
 
             if path.endswith("/"):
                 rel_file_path += "index.html"
             # Prevent directory traversal - normalize the path.
             rel_file_path = posixpath.normpath("/" + rel_file_path).lstrip("/")
             file_path = os.path.join(self.root, rel_file_path)
@@ -256,15 +262,15 @@
 
         # Wait until the ongoing rebuild (if any) finishes, so we're not serving a half-built site.
         with self._epoch_cond:
             self._epoch_cond.wait_for(lambda: self._visible_epoch == self._wanted_epoch)
             epoch = self._visible_epoch
 
         try:
-            file = open(file_path, "rb")
+            file: BinaryIO = open(file_path, "rb")
         except OSError:
             if not path.endswith("/") and os.path.isfile(os.path.join(file_path, "index.html")):
                 start_response("302 Found", [("Location", urllib.parse.quote(path) + "/")])
                 return []
             return None  # Not found
 
         if self._watched_paths and file_path.endswith(".html"):
@@ -297,14 +303,15 @@
         )
 
     @classmethod
     @functools.lru_cache()  # "Cache" to not repeat the same message for the same browser tab.
     def _log_poll_request(cls, url, request_id):
         log.info(f"Browser connected: {url}")
 
+    @classmethod
     def _guess_type(cls, path):
         # MkDocs only ensures a few common types (as seen in livereload_tests.py::test_mime_types).
         # Other uncommon types will not be accepted.
         if path.endswith((".js", ".JS")):
             return "application/javascript"
         if path.endswith(".gz"):
             return "application/gzip"
```

### Comparing `mkdocs-1.4.1/mkdocs/structure/files.py` & `mkdocs-1.4.2/mkdocs/structure/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,18 +226,15 @@
         return self.src_uri
 
     def _get_url(self, use_directory_urls: bool) -> str:
         """Return url based in destination path."""
         url = self.dest_uri
         dirname, filename = posixpath.split(url)
         if use_directory_urls and filename == 'index.html':
-            if dirname == '':
-                url = '.'
-            else:
-                url = dirname + '/'
+            url = (dirname or '.') + '/'
         return urlquote(url)
 
     def url_relative_to(self, other: File) -> str:
         """Return url for file relative to other file."""
         return utils.get_relative_url(self.url, other.url if isinstance(other, File) else other)
 
     def copy_file(self, dirty: bool = False) -> None:
```

### Comparing `mkdocs-1.4.1/mkdocs/structure/nav.py` & `mkdocs-1.4.2/mkdocs/structure/nav.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,21 +213,21 @@
         return Page(title, file, config)
     return Link(title, path)
 
 
 T = TypeVar('T')
 
 
-def _get_by_type(nav, T: Type[T]) -> List[T]:
+def _get_by_type(nav, t: Type[T]) -> List[T]:
     ret = []
     for item in nav:
-        if isinstance(item, T):
+        if isinstance(item, t):
             ret.append(item)
         if item.children:
-            ret.extend(_get_by_type(item.children, T))
+            ret.extend(_get_by_type(item.children, t))
     return ret
 
 
 def _add_parent_links(nav) -> None:
     for item in nav:
         if item.is_section:
             for child in item.children:
```

### Comparing `mkdocs-1.4.1/mkdocs/structure/pages.py` & `mkdocs-1.4.2/mkdocs/structure/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     meta: MutableMapping[str, Any]
     """A mapping of the metadata included at the top of the markdown page."""
 
     @property
     def url(self) -> str:
         """The URL of the page relative to the MkDocs `site_dir`."""
-        return '' if self.file.url == '.' else self.file.url
+        return '' if self.file.url in ('.', './') else self.file.url
 
     file: File
     """The documentation [`File`][mkdocs.structure.files.File] that the page is being rendered from."""
 
     abs_url: Optional[str]
     """The absolute URL of the page from the server root as determined by the value
     assigned to the [site_url][] configuration setting. The value includes any
@@ -129,15 +129,15 @@
     """The full URL to the source page in the source repository. Typically used to
     provide a link to edit the source page. [base_url][] should not be used with this
     variable."""
 
     @property
     def is_homepage(self) -> bool:
         """Evaluates to `True` for the homepage of the site and `False` for all other pages."""
-        return self.is_top_level and self.is_index and self.file.url in ['.', 'index.html']
+        return self.is_top_level and self.is_index and self.file.url in ('.', './', 'index.html')
 
     previous_page: Optional[Page]
     """The [page][mkdocs.structure.pages.Page] object for the previous page or `None`.
     The value will be `None` if the current page is the first item in the site navigation
     or if the current page is not included in the navigation at all."""
 
     next_page: Optional[Page]
```

### Comparing `mkdocs-1.4.1/mkdocs/structure/toc.py` & `mkdocs-1.4.2/mkdocs/structure/toc.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/base.py` & `mkdocs-1.4.2/mkdocs/tests/base.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/build_tests.py` & `mkdocs-1.4.2/mkdocs/tests/build_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/cli_tests.py` & `mkdocs-1.4.2/mkdocs/tests/cli_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/gh_deploy_tests.py` & `mkdocs-1.4.2/mkdocs/tests/gh_deploy_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/integration.py` & `mkdocs-1.4.2/mkdocs/tests/integration.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/livereload_tests.py` & `mkdocs-1.4.2/mkdocs/tests/livereload_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/localization_tests.py` & `mkdocs-1.4.2/mkdocs/tests/localization_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/new_tests.py` & `mkdocs-1.4.2/mkdocs/tests/new_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/plugin_tests.py` & `mkdocs-1.4.2/mkdocs/tests/plugin_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/search_tests.py` & `mkdocs-1.4.2/mkdocs/tests/search_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/theme_tests.py` & `mkdocs-1.4.2/mkdocs/tests/theme_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/config/base_tests.py` & `mkdocs-1.4.2/mkdocs/tests/config/base_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         os.mkdir(os.path.join(temp_dir, 'docs'))
 
         with self.assertLogs('mkdocs') as cm:
             with self.assertRaises(exceptions.Abort):
                 base.load_config(config_file=config_file.name)
         self.assertEqual(
             '\n'.join(cm.output),
-            "ERROR:mkdocs.config:Config value: 'site_name'. Error: Required configuration not provided.",
+            "ERROR:mkdocs.config:Config value 'site_name': Required configuration not provided.",
         )
 
     def test_pre_validation_error(self):
         class InvalidConfigOption(c.BaseConfigOption):
             def pre_validation(self, config, key_name):
                 raise ValidationError('pre_validation error')
 
@@ -202,15 +202,15 @@
 
         self.assertEqual(
             errors,
             [
                 ('invalid_option', ValidationError('pre_validation error')),
                 ('invalid_option', ValidationError('run_validation error')),
             ],
-        ),
+        )
         self.assertEqual(warnings, [])
 
     def test_run_and_post_validation_errors(self):
         """A run_validation error stops post_validation from running."""
 
         class InvalidConfigOption(c.BaseConfigOption):
             def run_validation(self, value):
```

### Comparing `mkdocs-1.4.1/mkdocs/tests/config/config_options_legacy_tests.py` & `mkdocs-1.4.2/mkdocs/tests/config/config_options_legacy_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             d = c.Deprecated()
 
         self.get_config(
             Schema,
             {'d': 'value'},
             warnings=dict(
                 d="The configuration option 'd' has been deprecated and will be removed in a "
-                "future release of MkDocs."
+                "future release."
             ),
         )
 
     def test_deprecated_option_message(self):
         class Schema:
             d = c.Deprecated(message='custom message for {} key')
 
@@ -205,29 +205,29 @@
             d = c.Deprecated(option_type=c.Type(str))
 
         self.get_config(
             Schema,
             {'d': 'value'},
             warnings=dict(
                 d="The configuration option 'd' has been deprecated and will be removed in a "
-                "future release of MkDocs."
+                "future release."
             ),
         )
 
     def test_deprecated_option_with_invalid_type(self):
         class Schema:
             d = c.Deprecated(option_type=c.Type(list))
 
         with self.expect_error(d="Expected type: <class 'list'> but received: <class 'str'>"):
             self.get_config(
                 Schema,
                 {'d': 'value'},
                 warnings=dict(
                     d="The configuration option 'd' has been deprecated and will be removed in a "
-                    "future release of MkDocs."
+                    "future release."
                 ),
             )
 
     def test_removed_option(self):
         class Schema:
             d = c.Deprecated(removed=True, moved_to='foo')
 
@@ -248,45 +248,45 @@
             old = c.Deprecated(moved_to='new')
 
         conf = self.get_config(
             Schema,
             {'old': 'value'},
             warnings=dict(
                 old="The configuration option 'old' has been deprecated and will be removed in a "
-                "future release of MkDocs. Use 'new' instead."
+                "future release. Use 'new' instead."
             ),
         )
         self.assertEqual(conf, {'new': 'value', 'old': None})
 
     def test_deprecated_option_move_complex(self):
         class Schema:
             foo = c.Type(dict)
             old = c.Deprecated(moved_to='foo.bar')
 
         conf = self.get_config(
             Schema,
             {'old': 'value'},
             warnings=dict(
                 old="The configuration option 'old' has been deprecated and will be removed in a "
-                "future release of MkDocs. Use 'foo.bar' instead."
+                "future release. Use 'foo.bar' instead."
             ),
         )
         self.assertEqual(conf, {'foo': {'bar': 'value'}, 'old': None})
 
     def test_deprecated_option_move_existing(self):
         class Schema:
             foo = c.Type(dict)
             old = c.Deprecated(moved_to='foo.bar')
 
         conf = self.get_config(
             Schema,
             {'old': 'value', 'foo': {'existing': 'existing'}},
             warnings=dict(
                 old="The configuration option 'old' has been deprecated and will be removed in a "
-                "future release of MkDocs. Use 'foo.bar' instead."
+                "future release. Use 'foo.bar' instead."
             ),
         )
         self.assertEqual(conf, {'foo': {'existing': 'existing', 'bar': 'value'}, 'old': None})
 
     def test_deprecated_option_move_invalid(self):
         class Schema:
             foo = c.Type(dict)
@@ -294,15 +294,15 @@
 
         with self.expect_error(foo="Expected type: <class 'dict'> but received: <class 'str'>"):
             self.get_config(
                 Schema,
                 {'old': 'value', 'foo': 'wrong type'},
                 warnings=dict(
                     old="The configuration option 'old' has been deprecated and will be removed in a "
-                    "future release of MkDocs. Use 'foo.bar' instead."
+                    "future release. Use 'foo.bar' instead."
                 ),
             )
 
 
 class IpAddressTest(TestCase):
     class Schema:
         option = c.IpAddress()
@@ -1197,39 +1197,39 @@
                 ):
                     self.get_config(Schema, {'option': val})
 
     def test_subconfig_ignored(self):
         """Default behaviour of subconfig: validation is ignored"""
 
         # Nominal
-        class Schema:
+        class Schema1:
             option = c.SubConfig(('cc', c.Choice(('foo', 'bar'))))
 
-        conf = self.get_config(Schema, {'option': {'cc': 'foo'}})
+        conf = self.get_config(Schema1, {'option': {'cc': 'foo'}})
         self.assertEqual(conf, {'option': {'cc': 'foo'}})
 
         # Invalid option: No error
-        class Schema:
+        class Schema2:
             option = c.SubConfig(('cc', c.Choice(('foo', 'bar'))))
 
-        conf = self.get_config(Schema, {'option': {'cc': True}})
+        conf = self.get_config(Schema2, {'option': {'cc': True}})
         self.assertEqual(conf, {'option': {'cc': True}})
 
         # Missing option: Will be considered optional with default None
-        class Schema:
+        class Schema3:
             option = c.SubConfig(('cc', c.Choice(('foo', 'bar'))))
 
-        conf = self.get_config(Schema, {'option': {}})
+        conf = self.get_config(Schema3, {'option': {}})
         self.assertEqual(conf, {'option': {'cc': None}})
 
         # Unknown option: No warning
-        class Schema:
+        class Schema4:
             option = c.SubConfig(('cc', c.Choice(('foo', 'bar'))))
 
-        conf = self.get_config(Schema, {'option': {'unknown_key_is_ok': 0}})
+        conf = self.get_config(Schema4, {'option': {'unknown_key_is_ok': 0}})
         self.assertEqual(conf, {'option': {'cc': None, 'unknown_key_is_ok': 0}})
 
     def test_subconfig_unknown_option(self):
         class Schema:
             option = c.SubConfig(validate=True)
 
         conf = self.get_config(
@@ -1243,15 +1243,15 @@
         class Schema:
             option = c.SubConfig(
                 ('cc', c.Choice(('foo', 'bar'))),
                 validate=True,
             )
 
         with self.expect_error(
-            option="Sub-option 'cc' configuration error: Expected one of: ('foo', 'bar') but received: True"
+            option="Sub-option 'cc': Expected one of: ('foo', 'bar') but received: True"
         ):
             self.get_config(Schema, {'option': {'cc': True}})
 
     def test_subconfig_normal(self):
         class Schema:
             option = c.SubConfig(
                 ('cc', c.Choice(('foo', 'bar'))),
@@ -1316,32 +1316,30 @@
         with self.expect_error(sub="Required configuration not provided."):
             conf = self.get_config(Schema, {})
 
         with self.expect_error(sub="Required configuration not provided."):
             conf = self.get_config(Schema, {'sub': None})
 
         with self.expect_error(
-            sub="Sub-option 'opt' configuration error: Expected type: <class 'int'> but received: <class 'str'>"
+            sub="Sub-option 'opt': Expected type: <class 'int'> but received: <class 'str'>"
         ):
             conf = self.get_config(Schema, {'sub': [{'opt': 'asdf'}, {}]})
 
         conf = self.get_config(Schema, {'sub': []})
 
         conf = self.get_config(Schema, {'sub': [{'opt': 1}, {'opt': 2}]})
         self.assertEqual(conf['sub'], [{'opt': 1}, {'opt': 2}])
 
         with self.expect_error(
-            sub="Sub-option 'opt' configuration error: Expected type: <class 'int'> but "
-            "received: <class 'str'>"
+            sub="Sub-option 'opt': Expected type: <class 'int'> but received: <class 'str'>"
         ):
             self.get_config(Schema, {'sub': [{'opt': 'z'}, {'opt': 2}]})
 
         with self.expect_error(
-            sub="Sub-option 'opt' configuration error: "
-            "Expected type: <class 'int'> but received: <class 'str'>"
+            sub="Sub-option 'opt': Expected type: <class 'int'> but received: <class 'str'>"
         ):
             conf = self.get_config(Schema, {'sub': [{'opt': 'z'}, {'opt': 2}]})
 
         with self.expect_error(
             sub="The configuration is invalid. The expected type was a key value mapping "
             "(a python dict) but we got an object of type: <class 'int'>"
         ):
```

### Comparing `mkdocs-1.4.1/mkdocs/tests/config/config_options_tests.py` & `mkdocs-1.4.2/mkdocs/tests/config/config_options_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             d = c.Deprecated()
 
         self.get_config(
             Schema,
             {'d': 'value'},
             warnings=dict(
                 d="The configuration option 'd' has been deprecated and will be removed in a "
-                "future release of MkDocs."
+                "future release."
             ),
         )
 
     def test_deprecated_option_message(self) -> None:
         class Schema(Config):
             d = c.Deprecated(message='custom message for {} key')
 
@@ -186,29 +186,29 @@
             d = c.Deprecated(option_type=c.Type(str))
 
         self.get_config(
             Schema,
             {'d': 'value'},
             warnings=dict(
                 d="The configuration option 'd' has been deprecated and will be removed in a "
-                "future release of MkDocs."
+                "future release."
             ),
         )
 
     def test_deprecated_option_with_invalid_type(self) -> None:
         class Schema(Config):
             d = c.Deprecated(option_type=c.Type(list))
 
         with self.expect_error(d="Expected type: <class 'list'> but received: <class 'str'>"):
             self.get_config(
                 Schema,
                 {'d': 'value'},
                 warnings=dict(
                     d="The configuration option 'd' has been deprecated and will be removed in a "
-                    "future release of MkDocs."
+                    "future release."
                 ),
             )
 
     def test_removed_option(self) -> None:
         class Schema(Config):
             d = c.Deprecated(removed=True, moved_to='foo')
 
@@ -229,45 +229,45 @@
             old = c.Deprecated(moved_to='new')
 
         conf = self.get_config(
             Schema,
             {'old': 'value'},
             warnings=dict(
                 old="The configuration option 'old' has been deprecated and will be removed in a "
-                "future release of MkDocs. Use 'new' instead."
+                "future release. Use 'new' instead."
             ),
         )
         self.assertEqual(conf, {'new': 'value', 'old': None})
 
     def test_deprecated_option_move_complex(self) -> None:
         class Schema(Config):
             foo = c.Type(dict)
             old = c.Deprecated(moved_to='foo.bar')
 
         conf = self.get_config(
             Schema,
             {'old': 'value'},
             warnings=dict(
                 old="The configuration option 'old' has been deprecated and will be removed in a "
-                "future release of MkDocs. Use 'foo.bar' instead."
+                "future release. Use 'foo.bar' instead."
             ),
         )
         self.assertEqual(conf, {'foo': {'bar': 'value'}, 'old': None})
 
     def test_deprecated_option_move_existing(self) -> None:
         class Schema(Config):
             foo = c.Type(dict)
             old = c.Deprecated(moved_to='foo.bar')
 
         conf = self.get_config(
             Schema,
             {'old': 'value', 'foo': {'existing': 'existing'}},
             warnings=dict(
                 old="The configuration option 'old' has been deprecated and will be removed in a "
-                "future release of MkDocs. Use 'foo.bar' instead."
+                "future release. Use 'foo.bar' instead."
             ),
         )
         self.assertEqual(conf, {'foo': {'existing': 'existing', 'bar': 'value'}, 'old': None})
 
     def test_deprecated_option_move_invalid(self) -> None:
         class Schema(Config):
             foo = c.Type(dict)
@@ -275,15 +275,15 @@
 
         with self.expect_error(foo="Expected type: <class 'dict'> but received: <class 'str'>"):
             self.get_config(
                 Schema,
                 {'old': 'value', 'foo': 'wrong type'},
                 warnings=dict(
                     old="The configuration option 'old' has been deprecated and will be removed in a "
-                    "future release of MkDocs. Use 'foo.bar' instead."
+                    "future release. Use 'foo.bar' instead."
                 ),
             )
 
 
 class IpAddressTest(TestCase):
     class Schema(Config):
         option = c.IpAddress()
@@ -1248,15 +1248,15 @@
         class Sub(Config):
             cc = c.Choice(('foo', 'bar'))
 
         class Schema(Config):
             option = c.SubConfig(Sub)
 
         with self.expect_error(
-            option="Sub-option 'cc' configuration error: Expected one of: ('foo', 'bar') but received: True"
+            option="Sub-option 'cc': Expected one of: ('foo', 'bar') but received: True"
         ):
             self.get_config(Schema, {'option': {'cc': True}})
 
     def test_subconfig_normal(self) -> None:
         class Sub(Config):
             cc = c.Choice(('foo', 'bar'))
 
@@ -1326,35 +1326,33 @@
         with self.expect_error(sub="Required configuration not provided."):
             conf = self.get_config(Schema, {})
 
         with self.expect_error(sub="Required configuration not provided."):
             conf = self.get_config(Schema, {'sub': None})
 
         with self.expect_error(
-            sub="Sub-option 'opt' configuration error: Expected type: <class 'int'> but received: <class 'str'>"
+            sub="Sub-option 'opt': Expected type: <class 'int'> but received: <class 'str'>"
         ):
             conf = self.get_config(Schema, {'sub': [{'opt': 'asdf'}, {}]})
 
         conf = self.get_config(Schema, {'sub': []})
 
         conf = self.get_config(Schema, {'sub': [{'opt': 1}, {'opt': 2}]})
         assert_type(conf.sub, List[Sub])
         self.assertEqual(conf.sub, [{'opt': 1}, {'opt': 2}])
         assert_type(conf.sub[0].opt, int)
         self.assertEqual(conf.sub[0].opt, 1)
 
         with self.expect_error(
-            sub="Sub-option 'opt' configuration error: Expected type: <class 'int'> but "
-            "received: <class 'str'>"
+            sub="Sub-option 'opt': Expected type: <class 'int'> but received: <class 'str'>"
         ):
             self.get_config(Schema, {'sub': [{'opt': 'z'}, {'opt': 2}]})
 
         with self.expect_error(
-            sub="Sub-option 'opt' configuration error: "
-            "Expected type: <class 'int'> but received: <class 'str'>"
+            sub="Sub-option 'opt': Expected type: <class 'int'> but received: <class 'str'>"
         ):
             conf = self.get_config(Schema, {'sub': [{'opt': 'z'}, {'opt': 2}]})
 
         with self.expect_error(
             sub="The configuration is invalid. The expected type was a key value mapping "
             "(a python dict) but we got an object of type: <class 'int'>"
         ):
@@ -1631,15 +1629,15 @@
 
 
 class _FakePlugin2Config(_FakePluginConfig):
     depr = c.Deprecated()
 
 
 class FakePlugin2(BasePlugin[_FakePlugin2Config]):
-    pass
+    supports_multiple_instances = True
 
 
 class ThemePlugin(BasePlugin[_FakePluginConfig]):
     pass
 
 
 class ThemePlugin2(BasePlugin[_FakePluginConfig]):
@@ -1802,14 +1800,65 @@
 
         cfg = {'plugins': ['/overridden']}
         conf = self.get_config(Schema, cfg)
 
         self.assertEqual(set(conf.plugins), {'overridden'})
         self.assertIsInstance(conf.plugins['overridden'], FakePlugin2)
 
+    def test_plugin_config_with_multiple_instances(self, mock_class) -> None:
+        class Schema(Config):
+            theme = c.Theme(default='mkdocs')
+            plugins = c.Plugins(theme_key='theme')
+
+        cfg = {
+            'plugins': [
+                {'sample2': {'foo': 'foo value', 'bar': 42}},
+                {'sample2': {'foo': 'foo2 value'}},
+            ],
+        }
+        conf = self.get_config(Schema, cfg)
+
+        self.assertEqual(
+            set(conf.plugins),
+            {'sample2', 'sample2 #2'},
+        )
+        self.assertEqual(conf.plugins['sample2'].config['bar'], 42)
+        self.assertEqual(conf.plugins['sample2 #2'].config['bar'], 0)
+
+    def test_plugin_config_with_multiple_instances_and_warning(self, mock_class) -> None:
+        class Schema(Config):
+            theme = c.Theme(default='mkdocs')
+            plugins = c.Plugins(theme_key='theme')
+
+        test_cfgs: List[Dict[str, Any]] = [
+            {
+                'theme': 'readthedocs',
+                'plugins': [{'sub_plugin': {}}, {'sample2': {}}, {'sub_plugin': {}}, 'sample2'],
+            },
+            {
+                'theme': 'readthedocs',
+                'plugins': ['sub_plugin', 'sample2', 'sample2', 'sub_plugin'],
+            },
+        ]
+
+        for cfg in test_cfgs:
+            conf = self.get_config(
+                Schema,
+                cfg,
+                warnings=dict(
+                    plugins="Plugin 'readthedocs/sub_plugin' was specified multiple times - "
+                    "this is likely a mistake, because the plugin doesn't declare "
+                    "`supports_multiple_instances`."
+                ),
+            )
+            self.assertEqual(
+                set(conf.plugins),
+                {'readthedocs/sub_plugin', 'readthedocs/sub_plugin #2', 'sample2', 'sample2 #2'},
+            )
+
     def test_plugin_config_empty_list_with_empty_default(self, mock_class) -> None:
         class Schema(Config):
             plugins = c.Plugins(default=[])
 
         cfg: Dict[str, Any] = {'plugins': []}
         conf = self.get_config(Schema, cfg)
 
@@ -1923,15 +1972,15 @@
 
         cfg = {
             'plugins': {
                 'sample': {'bar': 'not an int'},
             }
         }
         with self.expect_error(
-            plugins="Plugin 'sample' value: 'bar'. Error: Expected type: <class 'int'> but received: <class 'str'>"
+            plugins="Plugin 'sample' option 'bar': Expected type: <class 'int'> but received: <class 'str'>"
         ):
             self.get_config(Schema, cfg)
 
     def test_plugin_config_sub_warning(self, mock_class) -> None:
         class Schema(Config):
             plugins = c.Plugins()
 
@@ -1940,16 +1989,16 @@
                 'sample2': {'depr': 'deprecated value'},
             }
         }
         conf = self.get_config(
             Schema,
             cfg,
             warnings=dict(
-                plugins="Plugin 'sample2' value: 'depr'. Warning: The configuration option "
-                "'depr' has been deprecated and will be removed in a future release of MkDocs."
+                plugins="Plugin 'sample2' option 'depr': The configuration option "
+                "'depr' has been deprecated and will be removed in a future release."
             ),
         )
 
         self.assertIsInstance(conf.plugins, PluginCollection)
         self.assertIn('sample2', conf.plugins)
```

### Comparing `mkdocs-1.4.1/mkdocs/tests/config/config_tests.py` & `mkdocs-1.4.2/mkdocs/tests/config/config_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/integration/complicated_config/mkdocs.yml` & `mkdocs-1.4.2/mkdocs/tests/integration/complicated_config/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/image.png` & `mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/integration/subpages/docs/sub1/image.png` & `mkdocs-1.4.2/mkdocs/tests/integration/subpages/docs/sub1/image.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/structure/file_tests.py` & `mkdocs-1.4.2/mkdocs/tests/structure/file_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,29 +164,29 @@
 
     def test_md_index_file_use_directory_urls(self):
         f = File('index.md', '/path/to/docs', '/path/to/site', use_directory_urls=True)
         self.assertEqual(f.src_uri, 'index.md')
         self.assertPathsEqual(f.abs_src_path, '/path/to/docs/index.md')
         self.assertEqual(f.dest_uri, 'index.html')
         self.assertPathsEqual(f.abs_dest_path, '/path/to/site/index.html')
-        self.assertEqual(f.url, '.')
+        self.assertEqual(f.url, './')
         self.assertEqual(f.name, 'index')
         self.assertTrue(f.is_documentation_page())
         self.assertFalse(f.is_static_page())
         self.assertFalse(f.is_media_file())
         self.assertFalse(f.is_javascript())
         self.assertFalse(f.is_css())
 
     def test_md_readme_index_file_use_directory_urls(self):
         f = File('README.md', '/path/to/docs', '/path/to/site', use_directory_urls=True)
         self.assertEqual(f.src_uri, 'README.md')
         self.assertPathsEqual(f.abs_src_path, '/path/to/docs/README.md')
         self.assertEqual(f.dest_uri, 'index.html')
         self.assertPathsEqual(f.abs_dest_path, '/path/to/site/index.html')
-        self.assertEqual(f.url, '.')
+        self.assertEqual(f.url, './')
         self.assertEqual(f.name, 'index')
         self.assertTrue(f.is_documentation_page())
         self.assertFalse(f.is_static_page())
         self.assertFalse(f.is_media_file())
         self.assertFalse(f.is_javascript())
         self.assertFalse(f.is_css())
 
@@ -442,15 +442,15 @@
             'foo/bar/baz/index.md',
             'foo.md',
             'foo/bar.md',
             'foo/bar/baz.md',
         ]
 
         to_file_urls = [
-            '.',
+            './',
             'foo/',
             'foo/bar/',
             'foo/bar/baz/',
             'foo/',
             'foo/bar/',
             'foo/bar/baz/',
         ]
@@ -489,26 +489,26 @@
             self.assertEqual(from_file.url, 'foo/img.jpg')
             self.assertEqual(file.url, to_file_urls[i])
             self.assertEqual(from_file.url_relative_to(file.url), expected[i])
             self.assertEqual(from_file.url_relative_to(file), expected[i])
 
         from_file = File('index.html', '/path/to/docs', '/path/to/site', use_directory_urls=True)
         expected = [
-            '.',  # . relative to .
-            '..',  # . relative to foo/
-            '../..',  # . relative to foo/bar/
-            '../../..',  # . relative to foo/bar/baz/
-            '..',  # . relative to foo
-            '../..',  # . relative to foo/bar
-            '../../..',  # . relative to foo/bar/baz
+            './',  # . relative to .
+            '../',  # . relative to foo/
+            '../../',  # . relative to foo/bar/
+            '../../../',  # . relative to foo/bar/baz/
+            '../',  # . relative to foo
+            '../../',  # . relative to foo/bar
+            '../../../',  # . relative to foo/bar/baz
         ]
 
         for i, filename in enumerate(to_files):
             file = File(filename, '/path/to/docs', '/path/to/site', use_directory_urls=True)
-            self.assertEqual(from_file.url, '.')
+            self.assertEqual(from_file.url, './')
             self.assertEqual(file.url, to_file_urls[i])
             self.assertEqual(from_file.url_relative_to(file.url), expected[i])
             self.assertEqual(from_file.url_relative_to(file), expected[i])
 
         from_file = File('file.md', '/path/to/docs', '/path/to/site', use_directory_urls=True)
         expected = [
             'file/',  # file relative to .
```

### Comparing `mkdocs-1.4.1/mkdocs/tests/structure/nav_tests.py` & `mkdocs-1.4.2/mkdocs/tests/structure/nav_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/structure/page_tests.py` & `mkdocs-1.4.2/mkdocs/tests/structure/page_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -655,15 +655,15 @@
             '<p><a href="non-index/">link</a></p>',  # No trailing /
         )
 
     @mock.patch('mkdocs.structure.pages.open', mock.mock_open(read_data='[link](index.md)'))
     def test_relative_html_link_index(self):
         self.assertEqual(
             self.get_rendered_result(['non-index.md', 'index.md']),
-            '<p><a href="..">link</a></p>',
+            '<p><a href="../">link</a></p>',
         )
 
     @mock.patch('mkdocs.structure.pages.open', mock.mock_open(read_data='[link](sub2/index.md)'))
     def test_relative_html_link_sub_index(self):
         self.assertEqual(
             self.get_rendered_result(['index.md', 'sub2/index.md']),
             '<p><a href="sub2/">link</a></p>',  # No trailing /
@@ -692,15 +692,15 @@
             '<p><a href="file%20name/">link</a></p>',
         )
 
     @mock.patch('mkdocs.structure.pages.open', mock.mock_open(read_data='[link](../index.md)'))
     def test_relative_html_link_parent_index(self):
         self.assertEqual(
             self.get_rendered_result(['sub2/non-index.md', 'index.md']),
-            '<p><a href="../..">link</a></p>',
+            '<p><a href="../../">link</a></p>',
         )
 
     @mock.patch(
         'mkdocs.structure.pages.open', mock.mock_open(read_data='[link](non-index.md#hash)')
     )
     def test_relative_html_link_hash(self):
         self.assertEqual(
```

### Comparing `mkdocs-1.4.1/mkdocs/tests/structure/toc_tests.py` & `mkdocs-1.4.2/mkdocs/tests/structure/toc_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/utils/babel_stub_tests.py` & `mkdocs-1.4.2/mkdocs/tests/utils/babel_stub_tests.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/tests/utils/utils_tests.py` & `mkdocs-1.4.2/mkdocs/tests/utils/utils_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import unittest
 from unittest import mock
 
 from mkdocs import exceptions, utils
 from mkdocs.structure.files import File
 from mkdocs.structure.pages import Page
 from mkdocs.tests.base import dedent, load_config, tempdir
+from mkdocs.utils import meta
 
 BASEYML = """
 INHERIT: parent.yml
 foo: bar
 baz:
     sub1: replaced
     sub3: new
@@ -547,29 +548,29 @@
             Tags: foo
             Tags: bar
 
             Doc body
             """
         )
         self.assertEqual(
-            utils.meta.get_data(doc),
+            meta.get_data(doc),
             (
                 "Doc body",
                 {
                     'title': 'Foo Bar',
                     'date': '2018-07-10',
                     'summary': 'Line one Line two',
                     'tags': 'foo bar',
                 },
             ),
         )
 
     def test_mm_meta_data_blank_first_line(self):
         doc = '\nfoo: bar\nDoc body'
-        self.assertEqual(utils.meta.get_data(doc), (doc.lstrip(), {}))
+        self.assertEqual(meta.get_data(doc), (doc.lstrip(), {}))
 
     def test_yaml_meta_data(self):
         doc = dedent(
             """
             ---
             Title: Foo Bar
             Date: 2018-07-10
@@ -579,15 +580,15 @@
                 - foo
                 - bar
             ---
             Doc body
             """
         )
         self.assertEqual(
-            utils.meta.get_data(doc),
+            meta.get_data(doc),
             (
                 "Doc body",
                 {
                     'Title': 'Foo Bar',
                     'Date': datetime.date(2018, 7, 10),
                     'Summary': 'Line one Line two',
                     'Tags': ['foo', 'bar'],
@@ -600,34 +601,34 @@
             """
             ---
             - List item
             ---
             Doc body
             """
         )
-        self.assertEqual(utils.meta.get_data(doc), (doc, {}))
+        self.assertEqual(meta.get_data(doc), (doc, {}))
 
     def test_yaml_meta_data_invalid(self):
         doc = dedent(
             """
             ---
             foo: bar: baz
             ---
             Doc body
             """
         )
-        self.assertEqual(utils.meta.get_data(doc), (doc, {}))
+        self.assertEqual(meta.get_data(doc), (doc, {}))
 
     def test_no_meta_data(self):
         doc = dedent(
             """
             Doc body
             """
         )
-        self.assertEqual(utils.meta.get_data(doc), (doc, {}))
+        self.assertEqual(meta.get_data(doc), (doc, {}))
 
 
 class LogCounterTests(unittest.TestCase):
     def setUp(self):
         self.log = logging.getLogger('dummy')
         self.log.propagate = False
         self.log.setLevel(1)
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/base.html` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/keyboard-modal.html` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/keyboard-modal.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/messages.pot` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/messages.pot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/search-modal.html` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/search-modal.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/toc.html` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/toc.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/css/base.css` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/css/base.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/css/bootstrap.min.css` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/css/font-awesome.min.css` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/img/favicon.ico` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/img/grid.png` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/img/grid.png`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/js/base.js` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/js/base.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/js/bootstrap.min.js` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/js/jquery-1.10.2.min.js` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/js/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Marc Dietz <marc@projectleviathan.de>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "Aktion"
 
 msgid "Close"
 msgstr "Schließen"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Álvaro Mondéjar Rubio <mondejar1994@gmail.com>\n"
 "Language: es\n"
 "Language-Team: es\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "Acción"
 
 msgid "Close"
 msgstr "Cerrar"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Peyman Mohammadi <@peymanr34>\n"
 "Language: fa\n"
 "Language-Team: fa <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "عمل"
 
 msgid "Close"
 msgstr "بستن"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Alexys Jacob @ultrabug\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Close"
 msgstr "Fermer"
 
 msgid "Documentation built with %(mkdocs_link)s."
 msgstr "Documentation générée avec %(mkdocs_link)s."
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Francesco Maida <francesco.maida@gmail.com>\n"
 "Language: it\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "Azione"
 
 msgid "Close"
 msgstr "Chiudi"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Goto Hayato <habita.gh@gmail.com>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "アクション"
 
 msgid "Close"
 msgstr "閉じる"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Nicole Buitoni <ni.buitoni@gmail.com>\n"
 "Language: pt_BR\n"
 "Language-Team: pt_BR\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "Ação"
 
 msgid "Close"
 msgstr "Fechar"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: ru\n"
 "Language-Team: ru <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "Действие"
 
 msgid "Close"
 msgstr "Закрыть"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/tr_TR/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/tr_TR/LC_MESSAGES/messages.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Mustafa Sami Salt <mss1451@gmail.com>\n"
 "Language: tr_TR\n"
 "Language-Team: tr_TR <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "Eylem"
 
 msgid "Close"
 msgstr "Kapat"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/tr_TR/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/tr_TR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: uk\n"
 "Language-Team: uk <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "Дія"
 
 msgid "Close"
 msgstr "Закрити"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: xingkong0113 <dingpengyu06@gmail.com>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_Hans_CN <dingpengyu06@gmail.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Action"
 msgstr "动作"
 
 msgid "Close"
 msgstr "关闭"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/mkdocs/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/base.html` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/breadcrumbs.html` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/footer.html` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/footer.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/messages.pot` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/messages.pot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/nav.html` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/nav.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/search.html` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/versions.html` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/versions.html`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/theme.css` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/theme_extra.css` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/theme_extra.css`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/img/favicon.ico` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/js/html5shiv.min.js` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/js/theme.js` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/js/theme.js`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Marc Dietz <marc@projectleviathan.de>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "Breadcrumb-Navigation"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Álvaro Mondéjar Rubio <mondejar1994@gmail.com>\n"
 "Language: es\n"
 "Language-Team: es\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "Navegación de rastro"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Peyman Mohammadi <@peymanr34>\n"
 "Language: fa\n"
 "Language-Team: fa <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "فهرست مسیر"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Alexys Jacob @ultrabug\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "Fil d'Ariane"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Francesco Maida <francesco.maida@gmail.com>\n"
 "Language: it\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "Navigazione breadcrumb"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Goto Hayato <habita.gh@gmail.com>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "パンくずリストナビゲーション"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Gustavo Lucas Valente <gutivalente@gmail.com>\n"
 "Language: pt_BR\n"
 "Language-Team: pt_BR\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "Caminho de migalhas"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: ru\n"
 "Language-Team: ru\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "Навигационная цепочка"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/tr_TR/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/tr_TR/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: Mustafa Sami Salt <mss1451@gmail.com>\n"
 "Language: tr_TR\n"
 "Language-Team: tr_TR <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "Breadcrumb Gezinmesi"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/tr_TR/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/tr_TR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: uk\n"
 "Language-Team: uk <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "Навігаційна стежка"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr ""
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: xingkong0113 <dingpengyu06@gmail.com>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_Hans_CN <dingpengyu06@gmail.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "Breadcrumb Navigation"
 msgstr "面包屑导航"
 
 msgid ""
 "Built with %(mkdocs_link)s using a %(sphinx_link)s provided by %(rtd_link)s."
 msgstr "用%(mkdocs_link)s构建，使用%(rtd_link)s提供的%(sphinx_link)s。"
```

### Comparing `mkdocs-1.4.1/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po` & `mkdocs-1.4.2/mkdocs/themes/readthedocs/locales/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/utils/__init__.py` & `mkdocs-1.4.2/mkdocs/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 from collections import defaultdict
 from datetime import datetime, timezone
 from pathlib import PurePath
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
+    Collection,
     Dict,
     Iterable,
     List,
     MutableSequence,
     Optional,
     Tuple,
+    Type,
     TypeVar,
 )
 from urllib.parse import urlsplit
 
 if sys.version_info >= (3, 10):
     from importlib.metadata import EntryPoint, entry_points
 else:
@@ -70,15 +72,15 @@
     # Attach Environment Variable constructor.
     # See https://github.com/waylan/pyyaml-env-tag
     Loader.add_constructor('!ENV', construct_env_tag)
 
     return Loader
 
 
-def yaml_load(source: IO, loader=None) -> Optional[Dict[str, Any]]:
+def yaml_load(source: IO, loader: Optional[Type[yaml.Loader]] = None) -> Optional[Dict[str, Any]]:
     """Return dict of source YAML file using loader, recursively deep merging inherited parent."""
     Loader = loader or get_yaml_loader()
     result = yaml.load(source, Loader=Loader)
     if result is not None and 'INHERIT' in result:
         relpath = result.pop('INHERIT')
         abspath = os.path.normpath(os.path.join(os.path.dirname(source.name), relpath))
         if not os.path.exists(abspath):
@@ -362,15 +364,15 @@
             )
 
         themes[theme.name] = theme
 
     return themes
 
 
-def get_theme_names():
+def get_theme_names() -> Collection[str]:
     """Return a list of all installed themes by name."""
 
     return get_themes().keys()
 
 
 def dirname_to_title(dirname: str) -> str:
     """Return a page tile obtained from a directory name."""
```

### Comparing `mkdocs-1.4.1/mkdocs/utils/babel_stub.py` & `mkdocs-1.4.2/mkdocs/utils/babel_stub.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/mkdocs/utils/meta.py` & `mkdocs-1.4.2/mkdocs/utils/meta.py`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/.gitignore` & `mkdocs-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/LICENSE` & `mkdocs-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/README.md` & `mkdocs-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-1.4.1/pyproject.toml` & `mkdocs-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Documentation",
     "Topic :: Text Processing",
 ]
 dynamic = ["version"]
```

### Comparing `mkdocs-1.4.1/PKG-INFO` & `mkdocs-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs
-Version: 1.4.1
+Version: 1.4.2
 Summary: Project documentation with Markdown.
 Project-URL: Documentation, https://www.mkdocs.org/
 Project-URL: Source, https://github.com/mkdocs/mkdocs
 Project-URL: Issues, https://github.com/mkdocs/mkdocs/issues
 Project-URL: History, https://www.mkdocs.org/about/release-notes/
 Author-email: Tom Christie <tom@tomchristie.com>
 License-File: LICENSE
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.7
 Requires-Dist: click>=7.0
 Requires-Dist: colorama>=0.4; platform_system == 'Windows'
```

