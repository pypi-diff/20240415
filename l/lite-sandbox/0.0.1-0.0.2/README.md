# Comparing `tmp/lite-sandbox-0.0.1.tar.gz` & `tmp/lite-sandbox-0.0.2.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lite-sandbox-0.0.1.tar", last modified: Sun Apr 14 12:03:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

