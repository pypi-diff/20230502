# Comparing `tmp/rule_based_model-0.0.3.tar.gz` & `tmp/rule_based_model-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rule_based_model-0.0.3.tar", last modified: Mon May  1 20:22:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

