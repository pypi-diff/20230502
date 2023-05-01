# Comparing `tmp/FlipperNested-2.1.2.tar.gz` & `tmp/FlipperNested-2.2.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-2.1.2.tar", last modified: Sun Apr 30 14:45:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

