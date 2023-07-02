# Comparing `tmp/crystals-1.6.2.tar.gz` & `tmp/crystals-1.7.0a1-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crystals-1.6.2.tar", last modified: Fri Jan 13 13:53:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

