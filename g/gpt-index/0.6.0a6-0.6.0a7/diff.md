# Comparing `tmp/gpt_index-0.6.0a6.tar.gz` & `tmp/gpt_index-0.6.0a7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_index-0.6.0a6.tar", last modified: Tue May  2 07:45:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

