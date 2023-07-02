# Comparing `tmp/pyddm-0.6.1.tar.gz` & `tmp/pyddm-0.7.0-cp37-cp37m-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyddm-0.6.1.tar", last modified: Sun Jul 10 15:45:45 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

