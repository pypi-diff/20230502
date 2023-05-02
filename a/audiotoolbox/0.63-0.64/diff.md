# Comparing `tmp/audiotoolbox-0.63.tar.gz` & `tmp/audiotoolbox-0.64-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiotoolbox-0.63.tar", last modified: Thu Oct 20 08:18:28 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

