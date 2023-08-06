# Comparing `tmp/flask_unity-0.0.4.tar.gz` & `tmp/flask_unity-0.0.5-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_unity-0.0.4.tar", last modified: Sun Aug  6 23:01:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

