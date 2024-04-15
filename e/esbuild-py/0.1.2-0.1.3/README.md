# Comparing `tmp/esbuild_py-0.1.2.tar.gz` & `tmp/esbuild_py-0.1.3-cp37-cp37m-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esbuild_py-0.1.2.tar", last modified: Sun Apr 14 19:21:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

