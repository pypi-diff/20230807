# Comparing `tmp/django_query_tools-0.2.1.tar.gz` & `tmp/django_query_tools-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_query_tools-0.2.1.tar", last modified: Mon May 15 11:45:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

