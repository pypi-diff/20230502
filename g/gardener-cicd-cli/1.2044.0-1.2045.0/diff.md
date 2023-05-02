# Comparing `tmp/gardener-cicd-cli-1.2044.0.tar.gz` & `tmp/gardener_cicd_cli-1.2045.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2044.0.tar", last modified: Fri Apr 28 12:23:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

