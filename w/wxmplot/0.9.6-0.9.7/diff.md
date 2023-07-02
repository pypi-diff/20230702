# Comparing `tmp/wxmplot-0.9.6.tar.gz` & `tmp/wxmplot-0.9.7.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxmplot-0.9.6.tar", last modified: Mon Nov 21 19:26:24 2011, max compression, from Unix
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

