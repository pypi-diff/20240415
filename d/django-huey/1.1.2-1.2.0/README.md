# Comparing `tmp/django-huey-1.1.2.tar.gz` & `tmp/django_huey-1.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-huey-1.1.2.tar", last modified: Wed Nov  1 23:28:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

