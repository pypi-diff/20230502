# Comparing `tmp/chartfactor-4.1.5.tar.gz` & `tmp/chartfactor-4.1.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartfactor-4.1.5.tar", last modified: Wed Apr  5 20:32:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

