# Comparing `tmp/internetarchive-3.7.0.tar.gz` & `tmp/internetarchive-4.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetarchive-3.7.0.tar", last modified: Tue Mar 19 21:15:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
