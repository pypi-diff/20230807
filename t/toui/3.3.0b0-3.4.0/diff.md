# Comparing `tmp/toui-3.3.0b0.tar.gz` & `tmp/toui-3.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-3.3.0b0.tar", last modified: Sun Aug  6 07:56:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

