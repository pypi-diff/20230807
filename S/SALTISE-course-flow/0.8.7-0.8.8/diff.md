# Comparing `tmp/SALTISE_course_flow-0.8.7.tar.gz` & `tmp/SALTISE_course_flow-0.8.8.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SALTISE_course_flow-0.8.7.tar", last modified: Sat Jul 29 02:21:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

