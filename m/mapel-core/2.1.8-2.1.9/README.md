# Comparing `tmp/mapel-core-2.1.8.tar.gz` & `tmp/mapel_core-2.1.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-core-2.1.8.tar", last modified: Sat Mar 23 13:42:13 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

