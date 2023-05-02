# Comparing `tmp/volttron_dnp3_outstation-0.1.1a2.tar.gz` & `tmp/volttron_dnp3_outstation-0.1.1a3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_dnp3_outstation-0.1.1a2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

