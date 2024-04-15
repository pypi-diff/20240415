# Comparing `tmp/ATL_Tools-1.0.7.tar.gz` & `tmp/ATL_Tools-1.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATL_Tools-1.0.7.tar", last modified: Tue Apr  9 08:36:59 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

