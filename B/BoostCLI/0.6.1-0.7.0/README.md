# Comparing `tmp/boostcli-0.6.1.tar.gz` & `tmp/BoostCLI-0.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boostcli-0.6.1.tar", last modified: Sat Apr 13 22:24:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

