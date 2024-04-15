# Comparing `tmp/pymonetdb-1.7.1.tar.gz` & `tmp/pymonetdb-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonetdb-1.7.1.tar", last modified: Fri Sep 22 08:57:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
