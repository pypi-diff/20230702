# Comparing `tmp/blacksheep-2.0a7.tar.gz` & `tmp/blacksheep-2.0a8-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacksheep-2.0a7.tar", last modified: Wed May 31 06:10:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

