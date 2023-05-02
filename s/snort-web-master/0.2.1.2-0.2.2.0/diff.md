# Comparing `tmp/snort_web_master-0.2.1.2.tar.gz` & `tmp/snort_web_master-0.2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\snort_web_master-0.2.1.2.tar", last modified: Wed Apr 19 11:29:37 2023, max compression
+gzip compressed data, was "dist\snort_web_master-0.2.2.0.tar", last modified: Tue May  2 16:53:06 2023, max compression
```

## Comparing `snort_web_master-0.2.1.2.tar` & `snort_web_master-0.2.2.0.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.483942 snort_web_master-0.2.1.2/
--rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-0.2.1.2/LICENSE.rst
--rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-0.2.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      251 2023-04-19 11:29:37.483942 snort_web_master-0.2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-0.2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.374573 snort_web_master-0.2.1.2/data/
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.374573 snort_web_master-0.2.1.2/data/admin/
--rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.1.2/data/admin/0004_keyword_delete_keywords.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.390170 snort_web_master-0.2.1.2/data/admin/image/
--rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-0.2.1.2/data/admin/image/images.png
--rw-rw-rw-   0        0        0   241664 2023-01-07 17:05:37.000000 snort_web_master-0.2.1.2/data/db.sqlite3
--rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-0.2.1.2/data/dicts.py
--rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-0.2.1.2/data/dockercompose
--rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-0.2.1.2/data/favicon.ico
--rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-0.2.1.2/data/migrate sqllite to postgresql
--rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-0.2.1.2/data/my-snort-rule.tmp
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.405796 snort_web_master-0.2.1.2/data/nginx/
--rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-0.2.1.2/data/nginx/nginx
--rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-0.2.1.2/data/nginx/nginx.conf
--rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-0.2.1.2/data/requirements.txt
--rw-rw-rw-   0        0        0      793 2023-01-23 08:53:39.000000 snort_web_master-0.2.1.2/data/snortFile
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.249571 snort_web_master-0.2.1.2/data/templates/
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.405796 snort_web_master-0.2.1.2/data/templates/html/
--rw-rw-rw-   0        0        0     5678 2023-04-19 10:42:31.000000 snort_web_master-0.2.1.2/data/templates/html/full_rule.html
--rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-0.2.1.2/data/templates/html/import.html
--rw-rw-rw-   0        0        0    26921 2023-04-19 11:11:07.000000 snort_web_master-0.2.1.2/data/templates/html/snortBuilder.html
--rw-rw-rw-   0        0        0      140 2023-04-19 11:29:37.499545 snort_web_master-0.2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-04-19 11:28:23.000000 snort_web_master-0.2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.265170 snort_web_master-0.2.1.2/snort_web_master/
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.421420 snort_web_master-0.2.1.2/snort_web_master/pcaps/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/__init__.py
--rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.421420 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/
--rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0002_initial.py
--rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
--rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/__init__.py
--rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/models.py
--rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/tests.py
--rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-0.2.1.2/snort_web_master/pcaps/views.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.421420 snort_web_master-0.2.1.2/snort_web_master/settings/
--rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.2/snort_web_master/settings/__init__.py
--rw-rw-rw-   0        0        0      546 2023-04-19 09:25:30.000000 snort_web_master-0.2.1.2/snort_web_master/settings/admin.py
--rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.2/snort_web_master/settings/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.437046 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/
--rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
--rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0003_keywords_avalable.py
--rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
--rw-rw-rw-   0        0        0     1268 2023-04-19 09:28:30.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.1.2/snort_web_master/settings/migrations/__init__.py
--rw-rw-rw-   0        0        0     1444 2023-04-19 07:32:10.000000 snort_web_master-0.2.1.2/snort_web_master/settings/models.py
--rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.2/snort_web_master/settings/tests.py
--rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-0.2.1.2/snort_web_master/settings/views.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.437046 snort_web_master-0.2.1.2/snort_web_master/snort/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-0.2.1.2/snort_web_master/snort/__init__.py
--rw-rw-rw-   0        0        0    28285 2023-04-19 11:26:51.000000 snort_web_master-0.2.1.2/snort_web_master/snort/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-0.2.1.2/snort_web_master/snort/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.452670 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/
--rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0002_snortruleviewarray.py
--rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
--rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0004_snortrule_deleted.py
--rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
--rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
--rw-rw-rw-   0        0        0      477 2023-04-19 09:28:30.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0007_snortrule_tag.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.1.2/snort_web_master/snort/migrations/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-04-19 09:28:26.000000 snort_web_master-0.2.1.2/snort_web_master/snort/models.py
--rw-rw-rw-   0        0        0    19362 2023-01-12 18:25:18.000000 snort_web_master-0.2.1.2/snort_web_master/snort/parser.py
--rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-0.2.1.2/snort_web_master/snort/snort_templates.py
--rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-0.2.1.2/snort_web_master/snort/tests.py
--rw-rw-rw-   0        0        0     5584 2023-03-15 09:02:25.000000 snort_web_master-0.2.1.2/snort_web_master/snort/views.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.452670 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/
--rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/__init__.py
--rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/asgi.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.483942 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/middleware/
--rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/middleware/__init__.py
--rw-rw-rw-   0        0        0      537 2023-01-09 14:10:56.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/middleware/no_cache.py
--rw-rw-rw-   0        0        0     5515 2023-04-19 09:26:16.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/settings.py
--rw-rw-rw-   0        0        0     1959 2023-04-19 08:14:20.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/urls.py
--rw-rw-rw-   0        0        0      425 2023-04-19 08:13:33.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:29:37.483942 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/
--rw-rw-rw-   0        0        0      251 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3024 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-04-19 11:29:37.000000 snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.805821 snort_web_master-0.2.2.0/
+-rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-0.2.2.0/LICENSE.rst
+-rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-0.2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      251 2023-05-02 16:53:06.805821 snort_web_master-0.2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-0.2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.857864 snort_web_master-0.2.2.0/data/
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.894852 snort_web_master-0.2.2.0/data/admin/
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.2.0/data/admin/0004_keyword_delete_keywords.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.912848 snort_web_master-0.2.2.0/data/admin/image/
+-rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-0.2.2.0/data/admin/image/images.png
+-rw-rw-rw-   0        0        0   241664 2023-01-07 17:05:37.000000 snort_web_master-0.2.2.0/data/db.sqlite3
+-rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-0.2.2.0/data/dicts.py
+-rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-0.2.2.0/data/dockercompose
+-rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-0.2.2.0/data/favicon.ico
+-rw-rw-rw-   0        0        0    25803 2023-05-02 11:59:42.000000 snort_web_master-0.2.2.0/data/http.cap
+-rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-0.2.2.0/data/migrate sqllite to postgresql
+-rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-0.2.2.0/data/my-snort-rule.tmp
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.930860 snort_web_master-0.2.2.0/data/nginx/
+-rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-0.2.2.0/data/nginx/nginx
+-rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-0.2.2.0/data/nginx/nginx.conf
+-rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-0.2.2.0/data/requirements.txt
+-rw-rw-rw-   0        0        0      889 2023-05-02 14:51:31.000000 snort_web_master-0.2.2.0/data/snortFile
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.641309 snort_web_master-0.2.2.0/data/templates/
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.064855 snort_web_master-0.2.2.0/data/templates/html/
+-rw-rw-rw-   0        0        0     4867 2023-05-02 12:07:14.000000 snort_web_master-0.2.2.0/data/templates/html/full_rule.html
+-rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-0.2.2.0/data/templates/html/import.html
+-rw-rw-rw-   0        0        0    26921 2023-05-02 05:50:19.000000 snort_web_master-0.2.2.0/data/templates/html/snortBuilder.html
+-rw-rw-rw-   0        0        0      140 2023-05-02 16:53:06.807822 snort_web_master-0.2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-05-02 10:13:09.000000 snort_web_master-0.2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.646307 snort_web_master-0.2.2.0/snort_web_master/
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.109849 snort_web_master-0.2.2.0/snort_web_master/pcaps/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/__init__.py
+-rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.225077 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/
+-rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
+-rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/models.py
+-rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/tests.py
+-rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/views.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.277084 snort_web_master-0.2.2.0/snort_web_master/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.0/snort_web_master/settings/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-04-19 09:25:30.000000 snort_web_master-0.2.2.0/snort_web_master/settings/admin.py
+-rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.0/snort_web_master/settings/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.389279 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/
+-rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
+-rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0003_keywords_avalable.py
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
+-rw-rw-rw-   0        0        0     1268 2023-04-19 09:28:30.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-19 07:32:10.000000 snort_web_master-0.2.2.0/snort_web_master/settings/models.py
+-rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.0/snort_web_master/settings/tests.py
+-rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.0/snort_web_master/settings/views.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.518443 snort_web_master-0.2.2.0/snort_web_master/snort/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-0.2.2.0/snort_web_master/snort/__init__.py
+-rw-rw-rw-   0        0        0    31989 2023-05-02 16:50:50.000000 snort_web_master-0.2.2.0/snort_web_master/snort/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-0.2.2.0/snort_web_master/snort/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.628425 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/
+-rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0002_snortruleviewarray.py
+-rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
+-rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0004_snortrule_deleted.py
+-rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
+-rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
+-rw-rw-rw-   0        0        0      477 2023-04-19 09:28:30.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0007_snortrule_tag.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-04-19 09:28:26.000000 snort_web_master-0.2.2.0/snort_web_master/snort/models.py
+-rw-rw-rw-   0        0        0    19362 2023-01-12 18:25:18.000000 snort_web_master-0.2.2.0/snort_web_master/snort/parser.py
+-rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-0.2.2.0/snort_web_master/snort/snort_templates.py
+-rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-0.2.2.0/snort_web_master/snort/tests.py
+-rw-rw-rw-   0        0        0     5578 2023-05-02 16:32:07.000000 snort_web_master-0.2.2.0/snort_web_master/snort/views.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.748006 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/
+-rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/__init__.py
+-rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/asgi.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.803848 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/middleware/
+-rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/middleware/__init__.py
+-rw-rw-rw-   0        0        0      537 2023-01-09 14:10:56.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/middleware/no_cache.py
+-rw-rw-rw-   0        0        0     5515 2023-05-02 07:51:40.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/settings.py
+-rw-rw-rw-   0        0        0     1959 2023-04-19 08:14:20.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/urls.py
+-rw-rw-rw-   0        0        0      425 2023-04-19 08:13:33.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.778850 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3038 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/top_level.txt
```

### Comparing `snort_web_master-0.2.1.2/README.md` & `snort_web_master-0.2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/data/admin/0004_keyword_delete_keywords.py` & `snort_web_master-0.2.2.0/data/admin/0004_keyword_delete_keywords.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/data/admin/image/images.png` & `snort_web_master-0.2.2.0/data/admin/image/images.png`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/data/db.sqlite3` & `snort_web_master-0.2.2.0/data/db.sqlite3`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/data/dicts.py` & `snort_web_master-0.2.2.0/data/dicts.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/data/dockercompose` & `snort_web_master-0.2.2.0/data/dockercompose`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/data/favicon.ico` & `snort_web_master-0.2.2.0/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/data/migrate sqllite to postgresql` & `snort_web_master-0.2.2.0/data/migrate sqllite to postgresql`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/data/snortFile` & `snort_web_master-0.2.2.0/data/snortFile`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 RUN echo iptables-persistent iptables-persistent/autosave_v6 boolean true | debconf-set-selections
 RUN apt install python3 python3-pip iptables-persistent postgresql-client -y
 
 RUN python3 -m pip install --upgrade pip
 COPY requirements.txt requirements.txt
 RUN pip3 install -r requirements.txt
 
-COPY . .
+COPY ./snort_web_master .
 RUN mkdir -p /var/log/snort
 RUN touch /var/log/snort/alert
+RUN sed -i 's/--alert_fast = { }/--alert_fast = {stdout}/g' /home/snorty/snort3/etc/snort/snort.lua
 EXPOSE 8000
 ENV PATH="${PATH}:/home/snorty/snort3/bin/"
-ENTRYPOINT ["gunicorn", "snort_web_master.wsgi:application", "--bind", "0.0.0.0:8000"]
+ENTRYPOINT ["python3", "manage.py", "runserver", "0.0.0.0:8000"]
 # ENTRYPOINT /bin/bash
```

### Comparing `snort_web_master-0.2.1.2/data/templates/html/full_rule.html` & `snort_web_master-0.2.2.0/data/templates/html/full_rule.html`

 * *Files 22% similar despite different names*

```diff
@@ -42,92 +42,71 @@
   var group = document.getElementById("id_group")[document.getElementById("id_group").value];
   var name = document.getElementById("id_name").value;
   var id_document  = document.getElementById("id_document").value;
   var id_treatment = document.getElementById("id_treatment").value;
   var id_description = document.getElementById("id_description").value;
   var id_tag = ""
   if (document.getElementById("id_tag").checked === true) {
-  var id_tag = " tag:session,10,packets;"
+  var id_tag = " tag:session,packets 10;"
   }
   content = "";
   current_content = "";
   prev = null;
+  let substringsArray = ["depth", "offset", "distance", "within", "fast_pattern", "fast_pattern_offset", "fast_pattern_length", "nocase","relative","established", "count", "seconds"]
   for (let elem of document.getElementById("ruleform").childNodes) {
         if (elem.nodeType === 3||elem.tagName === "BR" ||elem.tagName === "IMG") // text node
         {
             continue;
         }
         if (elem.tagName === "SELECT") // inner node
         {
-            if (prev !== null){
-            if (prev.tagName === "SELECT"){
-            content = content + ';';
-            }
-            }
+            let sep = "";
             if (elem.value === "-----"){
                 continue;
             }
-            if (content.endsWith(":;")){
-                    content = content.replaceAll(":;", ";")
-                }
-            if (content.endsWith(";;")){
-                content = content.replaceAll(";;", ";")
-            }
-            content = content + elem.options[elem.selectedIndex].text;
-            if (content.endsWith(";!")){
-                content = content.replaceAll(";!", ": !")
-            }
-            if (content.endsWith(";;")){
-                content = content.replaceAll(";;", ";")
+            else if (substringsArray.some(v => elem.value === v)){
+                sep = ", ";
             }
-            if (!(content.endsWith(";")) && (content !== current_content)){
-                content = content + ";"
-                current_content = content;
+            else if (content == ""){}
+            else if (elem.value == "!"){}
+            else {
+                sep = "; ";
             }
+
+            content = content + sep + elem.options[elem.selectedIndex].text;
+            current_content = content;
         }
-        if (elem.tagName === "INPUT") // inner node
+        else if (elem.tagName === "INPUT") // inner node
         {
             if (elem.value === "-----"){
             continue;
             }
-            if (content.endsWith(":;")){
-                    content = content.replaceAll(":;", ";")
-                }
-            if (content.endsWith(";;")){
-                content = content.replaceAll(";;", ";")
-            }
-            if (elem.id.startsWith("keyword_selection") && elem.id.endsWith("data") && content.endsWith("!;"))
+            if (elem.id.startsWith("keyword_selection") && elem.id.endsWith("data") && content.endsWith("!"))
             {
-                content = content.substring(0, content.length-1) + "'" +elem.value +"';";
+                content = content.substring(0, content.length-1) + ': !"' +elem.value + '"';
             }
             else if (elem.id.startsWith("keyword_selection") && elem.id.endsWith("data")){
-                 content = content.substring(0, content.length-1) + ": '" +elem.value +"';";
+                 content = content + ': "' +elem.value +'"';
            }
            else{
-               content = content.substring(0, content.length-1) + ':' +elem.value +';';
+               content = content + ': ' +elem.value +'';
            }
-            if (content.endsWith(";;")){
-                content = content.replaceAll(";;", ";")
-            }
-            if (!(content.endsWith(";")) && (content !== current_content)){
-                content = content + ";"
-                current_content = content;
-            }
+            current_content = content;
         }
         prev = elem;
     }
   if (document.getElementById("id_group")[document.getElementById("id_group").value]!==undefined)
   {
    group = group.text;
   }
   else
   {
   group = "";
   }
 
-    id_content.value = id_content.textContent=action + " " + protocol + " " + srcipallow + srcip +" " +srcportallow+
-    srcport + " " + direction + " " + dstipallow + dstip + " " + dstportallow + dstport
-     + "(msg:" + group + " " + name+ ";" + content+ "sid:" +sigid +"; metadata: employee '"+
-     user_name + "', group '" + group + "', name '" + name + "', treatment '" + id_treatment +
-      "', keywords 'None', date '"+date_now+"', document '" + id_document + "',description '"+id_description+"'; "+id_tag+")";
+    id_content.value = id_content.textContent=action + ' ' + protocol + ' ' + srcipallow + srcip +' ' +srcportallow+
+    srcport + ' ' + direction + ' ' + dstipallow + dstip + ' ' + dstportallow + dstport
+     + '(msg:"' + group + '" ' + name+ ';' + content+ '; sid:' +sigid +'; metadata: employee "'+
+     user_name + '", group "' + group + '", name "' + name + '", treatment "' + id_treatment +
+      '", keywords "None", date "'+date_now+'", document "' + id_document + '",description "'+id_description+'"; '+id_tag+')';
 };
 </script>
```

### Comparing `snort_web_master-0.2.1.2/data/templates/html/snortBuilder.html` & `snort_web_master-0.2.2.0/data/templates/html/snortBuilder.html`

 * *Files 2% similar despite different names*

```diff
@@ -544,27 +544,27 @@
  );
 
 function set_value(value, field){
     var c = document.getElementById(field).onchange
     var b = document.getElementById(field).onblur
     document.getElementById(field).onchange = undefined
     document.getElementById(field).onblur = undefined
-    document.getElementById(field).value = value.trim("'")
+    document.getElementById(field).value = value.trim('"')
     document.getElementById(field).onchange = c
     document.getElementById(field).onblur = b
 }
 
 function content_change(){
    var id_content = document.getElementById("id_content");
     postData("/build_rule/keyword_to_rule", {"fule_rule": id_content.value})
     .then((data) =>
     {
         var res_data_post = data
         for (const els of data.data){
-            selectElementManual(els.htmlId, els.value.trim("'"), els.typeOfItem, els.locationX, els.locationY);
+            selectElementManual(els.htmlId, els.value.trim('"'), els.typeOfItem, els.locationX, els.locationY);
         };
         if (data.metadata_description !== undefined){
             set_value(data.metadata_description,"id_description")
         };
         if (data.metadata_document !== undefined){
             set_value(data.metadata_document,"id_document")
         };
@@ -614,30 +614,30 @@
 function get_clone_rule(){
     id_content.value = sessionStorage.getItem("snort_content")
     set_content_change()
     while (document.getElementById("id_description")== undefined){
         setTimeout(() => { get_clone_rule();}, 100)
         return;
     }
-    document.getElementById("id_description").value = sessionStorage.getItem("snort_description").trim("'").trim("'");
+    document.getElementById("id_description").value = sessionStorage.getItem("snort_description").trim('"').trim('"');
     while (document.getElementById("id_name")== undefined){
         setTimeout(() => { get_clone_rule();}, 100)
         return;
     }
-    document.getElementById("id_name").value = sessionStorage.getItem("snort_name").trim("'").trim("'");
+    document.getElementById("id_name").value = sessionStorage.getItem("snort_name").trim('"').trim('"');
     while (document.getElementById("id_treatment")== undefined){
         setTimeout(() => { get_clone_rule();}, 100)
         return;
     }
-    document.getElementById("id_treatment").value = sessionStorage.getItem("snort_treatment").trim("'").trim("'");
+    document.getElementById("id_treatment").value = sessionStorage.getItem("snort_treatment").trim('"').trim('"');
     while (document.getElementById("id_document")== undefined){
         setTimeout(() => { get_clone_rule();}, 100)
         return;
     }
-    document.getElementById("id_document").value = sessionStorage.getItem("snort_document").trim("'").trim("'");
+    document.getElementById("id_document").value = sessionStorage.getItem("snort_document").trim('"').trim('"');
 
     sessionStorage.removeItem("snort_content");
     sessionStorage.removeItem("snort_name");
     sessionStorage.removeItem("snort_treatment");
     sessionStorage.removeItem("snort_document");
 }
```

### Comparing `snort_web_master-0.2.1.2/setup.py` & `snort_web_master-0.2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='snort_web_master',
-    version='0.2.1.2',
+    version='0.2.2.0',
     license='MoCorp',
     readme="README.md",
     author="meir dahan",
     author_email='1dahanmeir1@gmail.com',
     packages=find_packages('snort_web_master'),
     package_dir={'': 'snort_web_master'},
     url='https://github.com/mosheovadi1/snort-web-master',
```

### Comparing `snort_web_master-0.2.1.2/snort_web_master/pcaps/admin.py` & `snort_web_master-0.2.2.0/snort_web_master/pcaps/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0001_initial.py` & `snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0002_initial.py` & `snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py` & `snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py` & `snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/pcaps/models.py` & `snort_web_master-0.2.2.0/snort_web_master/pcaps/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/settings/admin.py` & `snort_web_master-0.2.2.0/snort_web_master/settings/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0001_initial.py` & `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py` & `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0003_keywords_avalable.py` & `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0003_keywords_avalable.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py` & `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py` & `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/settings/models.py` & `snort_web_master-0.2.2.0/snort_web_master/settings/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/admin.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import csv
 import time
 from io import StringIO
 from django.contrib import messages
 import re
 from import_export.admin import ImportExportModelAdmin
 from django import forms
+
+import pcaps.models
 from .models import SnortRule, SnortRuleViewArray, save_rule_to_s3, delete_rule_from_s3
 from .snort_templates import types_list
 from .parser import Parser
 from django.utils.encoding import smart_str
 from django.http.response import HttpResponse, HttpResponseRedirect
 from django.utils.html import mark_safe
 from django.db import transaction
@@ -88,14 +90,27 @@
                 try:
                     if keyword.objects.get(name=options[option][0]):
                         break
                 except:
                     pass
             else:
                 raise Exception("no content; please add at least one keyword")
+            if os.name != "nt":
+                cur_rule = SnortRule()
+                cur_rule.content = self.data.get("content")
+                cur_rule.location = self.data.get("location")
+                cur_rule.group = self.instance.group
+                cur_rule.id = self.data.get("id")
+                cur_rule.treatment = self.data.get("treatment")
+                cur_rule.name = self.data.get("name")
+                cur_rule.type = self.data.get("type")
+                cur_rule.user = getattr(self.current_user, self.current_user.USERNAME_FIELD)
+                cur_rule.document = self.data.get("document")
+                pacps = [pcaps.models.Pcap(pcap_file="pacp_repo/http.cap")]
+                validate_pcap_snort(pacps, cur_rule)
         except Exception as e:
             raise forms.ValidationError(e)
 
         return self.data["content"]
 
     def clean_location(self):
         try:
@@ -130,16 +145,43 @@
         cur_rule.group = self.instance.group
         cur_rule.id = self.data.get("id")
         cur_rule.treatment = self.data.get("treatment")
         cur_rule.name = self.data.get("name")
         cur_rule.type = self.data.get("type")
         cur_rule.user = getattr(self.current_user, self.current_user.USERNAME_FIELD)
         cur_rule.document = self.data.get("document")
+        min_allowed = 0
+        max_allowed = 0
+        try:
+            max_allowed = int(Setting.objects.get(**{"name": "MAX_SANITY_MATCH_ALLOWED"}).value)
+        except:
+            forms.ValidationError(str(Setting.objects.get(**{"name": "MAX_SANITY_MATCH_ALLOWED"})) + " for MAX_SANITY_MATCH_ALLOWED is not a valid int")
+            return
+        try:
+            min_allowed = int(Setting.objects.get(**{"name": "MIN_SANITY_MATCH_ALLOWED"}).value)
+        except:
+            forms.ValidationError(
+                    str(Setting.objects.get(**{"name": "MIN_SANITY_MATCH_ALLOWED"})) + " for MIN_SANITY_MATCH_ALLOWED is not a valid int")
+            return
+        count = validate_pcap_snort(self.cleaned_data.get("pcap_sanity_check"), cur_rule)
+        print(f"clean_pcap_sanity_check: {min_allowed} <= int({count}) <= {max_allowed}")
+        if min_allowed <= count <= max_allowed:
+            self.cleaned_data["admin_locked"] = False
+            self.instance.admin_locked = False
+            self.instance.save()
+            return self.cleaned_data["pcap_sanity_check"]
+        elif Setting.objects.get(**{"name": "FORCE_SANITY_CHECK"}).value == "True":
+            self.cleaned_data["admin_locked"] = True
+            self.instance.admin_locked = True
+            self.instance.save()
+            if self.cleaned_data["active"] == True:
+                if not self.current_user.is_staff and not self.current_user.is_superuser:
+                    raise forms.ValidationError(
+                        f"rule is admin locked due to high number of validations {count} > {max_allowed}, please contact admin or fix rule\n all changed of an admin locked rull must be approved by admin")
 
-        validate_pcap_snort(self.cleaned_data.get("pcap_sanity_check"), cur_rule)
         return self.cleaned_data["pcap_sanity_check"]
 
     # only admin can activate admin locked rule
     def clean_pcap_legal_check(self):
         # return self.cleaned_data.get("pcap_validation")
 
         if not self.cleaned_data.get("pcap_legal_check"):
@@ -157,29 +199,39 @@
         cur_rule.location = self.data.get("location")
         cur_rule.id = self.data.get("id")
         cur_rule.treatment = self.data.get("treatment")
         cur_rule.name = self.data.get("name")
         cur_rule.type = self.data.get("type")
         cur_rule.user = getattr(self.current_user, self.current_user.USERNAME_FIELD)
         cur_rule.document = self.data.get("document")
-
+        try:
+            max_allowed = int(Setting.objects.get(**{"name": "MAX_LEGAL_MATCH_ALLOWED"}).value)
+        except:
+            forms.ValidationError(str(Setting.objects.get(**{"name": "MAX_SANITY_MATCH_ALLOWED"})) + " for MAX_SANITY_MATCH_ALLOWED is not a valid int")
+            return
+        try:
+            min_allowed = int(Setting.objects.get(**{"name": "MIN_LEGAL_MATCH_ALLOWED"}).value)
+        except:
+            forms.ValidationError(
+                    str(Setting.objects.get(**{"name": "MIN_SANITY_MATCH_ALLOWED"})) + " for MIN_SANITY_MATCH_ALLOWED is not a valid int")
+            return
         count = validate_pcap_snort(self.cleaned_data.get("pcap_legal_check"), cur_rule)
-        max_allowd = self.cleaned_data["MAX_MATCH_ALLOWD"]
-        if int(count) > max_allowd:
+        print(f"clean_pcap_legal_check: {min_allowed} <= int({count}) <= {max_allowed}")
+        if min_allowed <= int(count) <= max_allowed:
+            self.cleaned_data["admin_locked"] = False
+            self.instance.admin_locked = False
+            self.instance.save()
+        else:
             self.cleaned_data["admin_locked"] = True
             self.instance.admin_locked = True
             self.instance.save()
             if self.cleaned_data["active"] == True:
                 if not self.current_user.is_staff and not self.current_user.is_superuser:
                     raise forms.ValidationError(
-                        f"rule is admin locked due to hige number of validations {count}, please contact admin or fix rule\n all changed of an admin locked rull must be approved by admin")
-        else:
-            self.cleaned_data["admin_locked"] = False
-            self.instance.admin_locked = False
-            self.instance.save()
+                        f"rule is admin locked due to high number of validations {count} > {max_allowed}, please contact admin or fix rule\n all changed of an admin locked rull must be approved by admin")
 
         return self.cleaned_data["pcap_legal_check"]
 
     def clean_active(self):
         if self.instance.active:
             return self.cleaned_data["active"]
         locked = False
@@ -287,38 +339,41 @@
                                .strip()
                                .lower())
 
     with open(rule.location + ".tmp", "w") as rule_file:
         rule_file.write(rule.content)
     failed = True
     for pcap in pcaps:
+        failed = False
         try:
             base = "/app/"
             if os.name =="nt":
                 from django.conf import settings as s
                 base = str(s.BASE_DIR) + "/"
 
             if not verify_legal_pcap(f"{base}{pcap.pcap_file}"):
                 raise Exception(f"illegal pcap file")
             if not os.path.exists(f"{base}{pcap.pcap_file}"):
                 raise Exception(f"cant find file {base}{pcap.pcap_file}")
             stdout, stderr = subprocess.Popen(
                 ["/home/snorty/snort3/bin/snort", "-R", rule.location + ".tmp", "-r", f"{base}{pcap.pcap_file}", "-A",
-                 "fast"], stdout=subprocess.PIPE,
+                 "fast", "-c", "/home/snorty/snort3/etc/snort/snort.lua"], stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE).communicate()
             if stdout and not stderr:
                 if b"total_alerts: " in stdout:
                     return stdout.split(b"total_alerts: ")[1].split(b"\n")[0]
                 else:
                     return 0
+            if stderr:
+                raise Exception(stderr)
         except Exception as e:
             raise forms.ValidationError(f"could not validate rule on {base}{pcap.pcap_file}: {e}", code=405)
     if failed:
         raise Exception("no rules was chosen")
-    return stdout
+    return 0
 
 
 
 
 
 @admin.register(SnortRule)
 class SnortRuleAdmin(DjangoObjectActions, AdminAdvancedFiltersMixin, ImportExportModelAdmin, admin.ModelAdmin):
@@ -567,14 +622,19 @@
         form.base_fields["pcap_sanity_check"].help_text = "Hold down “Control” to select more than one."
         form.base_fields["pcap_legal_check"].help_text = "Hold down “Control” to select more than one."
         atkgroup = form.base_fields["group"]
         atkgroup.widget.can_add_related = Setting.objects.get_or_create(**{"name": "atkgroup_can_add_related"})[0].value == "True"
         atkgroup.widget.can_change_related = Setting.objects.get_or_create(**{"name": "atkgroup_can_change_related"})[0].value == "True"
         atkgroup.widget.can_delete_related = Setting.objects.get_or_create(**{"name": "atkgroup_can_delete_related"})[0].value == "True"
         atkgroup.widget.can_view_related = Setting.objects.get_or_create(**{"name": "atkgroup_can_view_related"})[0].value == "True"
+        a = Setting.objects.get_or_create(**{"name": "MAX_SANITY_MATCH_ALLOWED"},defaults={"value": 1000})
+        if a[1]:
+            a = Setting.objects.get_or_create(**{"name": "MIN_SANITY_MATCH_ALLOWED"}, defaults={"value": 0})
+            a = Setting.objects.get_or_create(**{"name": "MAX_LEGAL_MATCH_ALLOWED"}, defaults={"value": 0})
+            a = Setting.objects.get_or_create(**{"name": "MIN_LEGAL_MATCH_ALLOWED"}, defaults={"value": 0})
         return form
 
     @transaction.atomic
     def clone_rule(self, request, obj: SnortRule):
         return HttpResponseRedirect(f"/snort/snortrule/add/")
 
     clone_rule.label = "clone_rule"  # optional
```

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0001_initial.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0002_snortruleviewarray.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0002_snortruleviewarray.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/models.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/parser.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/parser.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/snort_templates.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/snort_templates.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort/tests.py` & `snort_web_master-0.2.2.0/snort_web_master/snort/tests.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort_web_master/middleware/no_cache.py` & `snort_web_master-0.2.2.0/snort_web_master/snort_web_master/middleware/no_cache.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort_web_master/settings.py` & `snort_web_master-0.2.2.0/snort_web_master/snort_web_master/settings.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort_web_master/urls.py` & `snort_web_master-0.2.2.0/snort_web_master/snort_web_master/urls.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.1.2/snort_web_master/snort_web_master.egg-info/SOURCES.txt` & `snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.cfg
 setup.py
 data/db.sqlite3
 data/dicts.py
 data/dockercompose
 data/favicon.ico
+data/http.cap
 data/migrate sqllite to postgresql
 data/my-snort-rule.tmp
 data/requirements.txt
 data/snortFile
 data/admin/0004_keyword_delete_keywords.py
 data/admin/image/images.png
 data/nginx/nginx
```

