# Comparing `tmp/psycopg-3.1.8.tar.gz` & `tmp/psycopg-3.1.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg-3.1.8.tar", last modified: Mon Jan 16 22:56:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

