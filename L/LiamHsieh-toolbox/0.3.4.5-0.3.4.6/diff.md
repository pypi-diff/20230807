# Comparing `tmp/LiamHsieh toolbox-0.3.4.5.tar.gz` & `tmp/LiamHsieh_toolbox-0.3.4.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiamHsieh toolbox-0.3.4.5.tar", last modified: Wed Jun  7 23:48:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

