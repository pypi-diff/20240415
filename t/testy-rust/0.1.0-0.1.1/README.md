# Comparing `tmp/TestY_rust-0.1.0.tar.gz` & `tmp/TestY_rust-0.1.1-pp39-pypy39_pp73-musllinux_1_2_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

