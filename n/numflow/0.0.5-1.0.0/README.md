# Comparing `tmp/numflow-0.0.5.tar.gz` & `tmp/numflow-1.0.0-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/numflow-0.0.5.tar", last modified: Tue Jan 14 10:43:59 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

