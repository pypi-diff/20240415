# Comparing `tmp/fast_tradier_client-0.3.2.tar.gz` & `tmp/fast_tradier_client-0.3.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tradier_client-0.3.2.tar", last modified: Thu Feb  8 02:21:45 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

