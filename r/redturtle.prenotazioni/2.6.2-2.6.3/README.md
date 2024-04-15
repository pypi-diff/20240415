# Comparing `tmp/redturtle.prenotazioni-2.6.2.tar.gz` & `tmp/redturtle.prenotazioni-2.6.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.prenotazioni-2.6.2.tar", last modified: Fri Apr 12 11:59:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

