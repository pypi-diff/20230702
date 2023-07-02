# Comparing `tmp/backendpy-0.2.5a3.tar.gz` & `tmp/backendpy-0.2.5a4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backendpy-0.2.5a3.tar", last modified: Fri Jun 23 15:21:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

