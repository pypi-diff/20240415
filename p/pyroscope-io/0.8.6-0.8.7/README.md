# Comparing `tmp/pyroscope-io-0.8.6.tar.gz` & `tmp/pyroscope_io-0.8.7-py2.py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscope-io-0.8.6.tar", last modified: Mon Apr  8 04:42:20 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

