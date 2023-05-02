# Comparing `tmp/OctoBot-Tulipy-0.4.2.tar.gz` & `tmp/OctoBot_Tulipy-0.4.3-cp38-cp38-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Tulipy-0.4.2.tar", last modified: Thu Jan  6 06:52:37 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

