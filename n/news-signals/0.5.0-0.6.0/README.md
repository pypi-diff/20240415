# Comparing `tmp/news-signals-0.5.0.tar.gz` & `tmp/news_signals-0.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news-signals-0.5.0.tar", last modified: Fri Mar 29 08:01:58 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

