# Comparing `tmp/ul-api-utils-7.8.6.tar.gz` & `tmp/ul-api-utils-7.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-api-utils-7.8.6.tar", last modified: Fri Apr 12 14:13:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

