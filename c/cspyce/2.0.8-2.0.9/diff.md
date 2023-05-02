# Comparing `tmp/cspyce-2.0.8.tar.gz` & `tmp/cspyce-2.0.9-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cspyce-2.0.8.tar", last modified: Wed Apr 19 20:55:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

