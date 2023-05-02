# Comparing `tmp/jupyter_nbextensions_configurator-0.6.1.tar.gz` & `tmp/jupyter_nbextensions_configurator-0.6.2-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_nbextensions_configurator-0.6.1.tar", last modified: Tue Nov 15 16:24:14 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

