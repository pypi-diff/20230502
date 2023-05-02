# Comparing `tmp/pysui_sdk-1.0.0.tar.gz` & `tmp/pysui_sdk-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysui_sdk-1.0.0.tar", last modified: Tue May  2 05:25:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

