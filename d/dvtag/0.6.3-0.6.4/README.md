# Comparing `tmp/dvtag-0.6.3.tar.gz` & `tmp/dvtag-0.6.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvtag-0.6.3.tar", last modified: Wed Apr  3 08:02:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

