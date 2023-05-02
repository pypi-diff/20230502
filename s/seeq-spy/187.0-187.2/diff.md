# Comparing `tmp/seeq-spy-187.0.tar.gz` & `tmp/seeq_spy-187.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\seeq-spy-187.0.tar", last modified: Thu Apr 13 22:01:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

