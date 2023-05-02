# Comparing `tmp/crc-event-schemas-0.1.2.tar.gz` & `tmp/crc_event_schemas-0.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc-event-schemas-0.1.2.tar", last modified: Tue Apr 25 16:02:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

