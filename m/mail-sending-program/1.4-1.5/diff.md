# Comparing `tmp/mail sending program-1.4.tar.gz` & `tmp/mail_sending_program-1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mail sending program-1.4.tar", last modified: Fri Aug 13 15:48:11 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

