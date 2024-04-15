# Comparing `tmp/fugashi-1.3.1.dev0.tar.gz` & `tmp/fugashi-1.3.2.dev0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugashi-1.3.1.dev0.tar", last modified: Fri Mar  8 15:06:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

