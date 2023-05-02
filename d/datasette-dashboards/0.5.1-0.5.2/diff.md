# Comparing `tmp/datasette_dashboards-0.5.1.tar.gz` & `tmp/datasette_dashboards-0.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_dashboards-0.5.1.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

