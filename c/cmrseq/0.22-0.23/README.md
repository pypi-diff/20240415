# Comparing `tmp/cmrseq-0.22.tar.gz` & `tmp/cmrseq-0.23-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmrseq-0.22.tar", last modified: Wed May 31 14:47:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

