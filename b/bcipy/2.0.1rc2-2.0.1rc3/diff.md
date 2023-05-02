# Comparing `tmp/bcipy-2.0.1rc2.tar.gz` & `tmp/bcipy-2.0.1rc3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcipy-2.0.1rc2.tar", last modified: Fri Oct 14 22:23:29 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

