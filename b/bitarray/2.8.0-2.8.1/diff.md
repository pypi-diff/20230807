# Comparing `tmp/bitarray-2.8.0.tar.gz` & `tmp/bitarray-2.8.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitarray-2.8.0.tar", last modified: Sat Jul 22 05:53:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

