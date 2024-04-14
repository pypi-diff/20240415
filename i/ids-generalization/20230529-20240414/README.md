# Comparing `tmp/ids-generalization-20230529.tar.gz` & `tmp/ids_generalization-20240414-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ids-generalization-20230529.tar", last modified: Tue Nov  7 20:20:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

