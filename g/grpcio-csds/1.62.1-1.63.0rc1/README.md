# Comparing `tmp/grpcio-csds-1.62.1.tar.gz` & `tmp/grpcio_csds-1.63.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-csds-1.62.1.tar", last modified: Fri Mar  8 00:12:21 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
