# Comparing `tmp/flask_unity-0.0.7.tar.gz` & `tmp/flask_unity-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_unity-0.0.7.tar", last modified: Sun Aug  6 23:07:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

