# Comparing `tmp/cygrid-2.0.3.tar.gz` & `tmp/cygrid-2.0.4-cp38-cp38-manylinux_2_28_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cygrid-2.0.3.tar", last modified: Tue Nov 22 23:08:45 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

