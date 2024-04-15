# Comparing `tmp/cellmaps_utils-0.2.0.post1.tar.gz` & `tmp/cellmaps_utils-0.3.0a1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_utils-0.2.0.post1.tar", last modified: Wed Feb 28 22:25:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

