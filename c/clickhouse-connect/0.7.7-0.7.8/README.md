# Comparing `tmp/clickhouse-connect-0.7.7.tar.gz` & `tmp/clickhouse_connect-0.7.8-cp310-cp310-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.7.7.tar", last modified: Wed Apr  3 11:56:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

