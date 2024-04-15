# Comparing `tmp/serialtools-0.8.1.tar.gz` & `tmp/serialtools-0.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialtools-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

