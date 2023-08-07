# Comparing `tmp/openmetadata_managed_apis-1.1.0.4.tar.gz` & `tmp/openmetadata_managed_apis-1.1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmetadata_managed_apis-1.1.0.4.tar", last modified: Thu Jul 20 12:10:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

