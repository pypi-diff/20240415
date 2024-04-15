# Comparing `tmp/OSBModelValidation-0.2.19.tar.gz` & `tmp/OSBModelValidation-0.2.20-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OSBModelValidation-0.2.19.tar", last modified: Fri Apr 12 09:03:23 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

