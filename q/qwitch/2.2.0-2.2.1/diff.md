# Comparing `tmp/qwitch-2.2.0.tar.gz` & `tmp/qwitch-2.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwitch-2.2.0.tar", last modified: Mon May  1 17:05:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

