# Comparing `tmp/proceso-0.0.4.tar.gz` & `tmp/proceso-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proceso-0.0.4.tar", last modified: Tue May  2 01:51:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

