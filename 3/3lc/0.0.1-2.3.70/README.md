# Comparing `tmp/3lc-0.0.1.tar.gz` & `tmp/3lc-2.3.70-0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3lc-0.0.1.tar", last modified: Tue Aug 22 14:07:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

