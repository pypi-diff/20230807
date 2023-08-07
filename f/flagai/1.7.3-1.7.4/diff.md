# Comparing `tmp/flagai-1.7.3.tar.gz` & `tmp/flagai-1.7.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagai-1.7.3.tar", last modified: Wed Jun 14 07:39:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

