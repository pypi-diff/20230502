# Comparing `tmp/yeref-0.1.50.tar.gz` & `tmp/yeref-0.1.51-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.50.tar", last modified: Mon May  1 08:43:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

