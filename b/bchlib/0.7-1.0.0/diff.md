# Comparing `tmp/bchlib-0.7.tar.gz` & `tmp/bchlib-1.0.0-cp36-cp36m-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bchlib-0.7.tar", last modified: Thu May 17 22:14:38 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

