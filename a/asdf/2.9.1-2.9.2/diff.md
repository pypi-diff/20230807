# Comparing `tmp/asdf-2.9.1.tar.gz` & `tmp/asdf-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asdf-2.9.1.tar", last modified: Thu Feb  3 15:48:06 2022, max compression
+gzip compressed data, was "asdf-2.9.2.tar", last modified: Tue Feb  8 01:08:56 2022, max compression
```

## Comparing `asdf-2.9.1.tar` & `asdf-2.9.2.tar`

### file list

```diff
@@ -1,552 +1,553 @@
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.698868 asdf-2.9.1/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.328482 asdf-2.9.1/.github/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.347870 asdf-2.9.1/.github/workflows/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      541 2021-07-30 18:34:35.000000 asdf-2.9.1/.github/workflows/changelog.yml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3454 2022-02-01 15:44:28.000000 asdf-2.9.1/.github/workflows/ci.yml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2635 2022-02-03 15:47:44.000000 asdf-2.9.1/.github/workflows/downstream.yml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1174 2022-02-01 15:44:28.000000 asdf-2.9.1/.github/workflows/s390x.yml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    23045 2022-02-03 15:47:44.000000 asdf-2.9.1/CHANGES.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3246 2021-07-30 18:34:35.000000 asdf-2.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1035 2021-07-30 18:34:35.000000 asdf-2.9.1/CONTRIBUTING.md
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1539 2021-07-30 18:34:35.000000 asdf-2.9.1/LICENSE
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)       92 2021-07-30 18:34:35.000000 asdf-2.9.1/MANIFEST.in
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    11698 2022-02-03 15:48:06.699093 asdf-2.9.1/PKG-INFO
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    10762 2022-02-01 15:44:28.000000 asdf-2.9.1/README.rst
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.361408 asdf-2.9.1/asdf/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      740 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2025 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/_convenience.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    11445 2022-01-31 22:13:07.000000 asdf-2.9.1/asdf/_display.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      576 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/_helpers.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    66125 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/asdf.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      523 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/asdftypes.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    47971 2022-01-31 22:13:07.000000 asdf-2.9.1/asdf/block.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.612629 asdf-2.9.1/asdf/commands/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      592 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1966 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/defragment.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    12116 2021-12-27 14:46:55.000000 asdf-2.9.1/asdf/commands/diff.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    11646 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/edit.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3321 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/exploded.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2638 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/extension.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1595 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/extract.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1278 2021-06-02 16:03:49.000000 asdf-2.9.1/asdf/commands/info.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1967 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/main.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1364 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/remove_hdu.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1606 2022-01-31 22:13:07.000000 asdf-2.9.1/asdf/commands/tags.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.617873 asdf-2.9.1/asdf/commands/tests/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/__init__.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.629121 asdf-2.9.1/asdf/commands/tests/data/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/data/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    80469 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/commands/tests/data/block0.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    80469 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/commands/tests/data/block1.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      276 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/commands/tests/data/blocks.diff
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1246 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/commands/tests/data/frames.diff
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4191 2020-07-15 21:37:54.000000 asdf-2.9.1/asdf/commands/tests/data/frames0.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3793 2021-03-25 16:43:49.000000 asdf-2.9.1/asdf/commands/tests/data/frames1.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1160 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/data/frames_ignore_asdf_library.diff
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/data/frames_ignore_both.diff
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      103 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/data/frames_ignore_reference_frame.diff
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      269 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/commands/tests/data/frames_minimal.diff
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)       41 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/data/simple_inline_array.diff
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      495 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/data/simple_inline_array0.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      495 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/data/simple_inline_array1.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1367 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/test_defragment.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2320 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/test_diff.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     9360 2022-01-25 17:23:32.000000 asdf-2.9.1/asdf/commands/tests/test_edit.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1592 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/test_exploded.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      454 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/test_extension.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      984 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/test_extract.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1042 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/test_info.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      415 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/test_main.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      927 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/test_remove_hdu.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      598 2022-01-31 22:13:07.000000 asdf-2.9.1/asdf/commands/tests/test_tags.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      874 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/tests/test_to_yaml.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1936 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/commands/to_yaml.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.629987 asdf-2.9.1/asdf/compat/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/compat/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      176 2020-08-14 18:53:55.000000 asdf-2.9.1/asdf/compat/numpycompat.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    10430 2022-01-25 17:23:32.000000 asdf-2.9.1/asdf/compression.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    12169 2022-01-25 17:23:32.000000 asdf-2.9.1/asdf/config.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1276 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/conftest.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      649 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/constants.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2376 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/entry_points.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      528 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/exceptions.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.632898 asdf-2.9.1/asdf/extension/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      947 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/extension/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2543 2022-01-25 17:23:32.000000 asdf-2.9.1/asdf/extension/_compressor.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    11052 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/extension/_converter.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    10835 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/extension/_extension.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8031 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/extension/_legacy.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     6170 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/extension/_manager.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3510 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/extension/_manifest.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2571 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/extension/_tag.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.633816 asdf-2.9.1/asdf/extern/
--rwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)     7095 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/extern/RangeHTTPServer.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        8 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/extern/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4170 2020-09-21 19:09:31.000000 asdf-2.9.1/asdf/extern/atomicfile.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    12069 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/fits_embed.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    33320 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/generic_io.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5317 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/reference.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5854 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/resolver.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     9003 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/resource.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    26685 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/schema.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    12515 2022-02-01 15:44:29.000000 asdf-2.9.1/asdf/search.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1788 2022-01-05 19:54:57.000000 asdf-2.9.1/asdf/stream.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4269 2022-01-25 17:23:32.000000 asdf-2.9.1/asdf/tagged.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.634178 asdf-2.9.1/asdf/tags/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tags/__init__.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.635912 asdf-2.9.1/asdf/tags/core/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1641 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      531 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/complex.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      434 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/constant.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2185 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/external_reference.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3438 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/integer.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    25272 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/ndarray.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.638472 asdf-2.9.1/asdf/tags/core/tests/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tags/core/tests/__init__.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.639827 asdf-2.9.1/asdf/tags/core/tests/data/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tags/core/tests/data/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      473 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tags/core/tests/data/datatype-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      187 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tags/core/tests/data/ndim-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1365 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/tests/test_complex.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      636 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/tests/test_extension_metadata.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      340 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/tests/test_external_reference.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8452 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/tests/test_history.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2317 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tags/core/tests/test_integer.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    25698 2022-01-25 17:23:32.000000 asdf-2.9.1/asdf/tags/core/tests/test_ndarray.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.640795 asdf-2.9.1/asdf/testing/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/testing/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1555 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/testing/helpers.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.652235 asdf-2.9.1/asdf/tests/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1764 2021-12-27 14:46:55.000000 asdf-2.9.1/asdf/tests/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      736 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/conftest.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      608 2020-08-14 18:53:55.000000 asdf-2.9.1/asdf/tests/coveragerc
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.671397 asdf-2.9.1/asdf/tests/data/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/data/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3840 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/data/asdf.fits.gz
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      138 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/complex-42.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      149 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/custom-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      214 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/custom_flow-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      215 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/custom_flow-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      545 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/custom_schema.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      306 2020-08-14 18:53:55.000000 asdf-2.9.1/asdf/tests/data/custom_schema_definitions.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      395 2020-08-14 18:53:55.000000 asdf-2.9.1/asdf/tests/data/custom_schema_external_ref.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      158 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/custom_style-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1072 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/data/default-1.0.0.yaml
--rwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)     2203 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/example_schema.json
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8641 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/data/extension_check.fits
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      525 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/foreign_tag_reference-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      581 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/fraction-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      442 2020-08-14 18:53:55.000000 asdf-2.9.1/asdf/tests/data/fraction_with_inverse-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      355 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/fractional_2d_coord-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      137 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/missing-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      407 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/data/one_of-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      183 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/self_referencing-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      378 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/tag_reference-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5760 2020-05-18 17:01:06.000000 asdf-2.9.1/asdf/tests/data/version_mismatch.fits
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    15257 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/helpers.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2070 2022-01-31 22:13:07.000000 asdf-2.9.1/asdf/tests/httpserver.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    18332 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/test_api.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    24895 2022-01-25 17:23:32.000000 asdf-2.9.1/asdf/tests/test_array_blocks.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    11537 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/tests/test_asdf.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     7123 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/test_compression.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    12398 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/test_config.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4844 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_entry_points.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    24805 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/tests/test_extension.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5348 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_file_format.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    17630 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/test_fits_embed.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    24158 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_generic_io.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1153 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_helpers.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3438 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf/tests/test_integration.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8301 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_reference.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2484 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_reference_files.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3647 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_resolver.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    12114 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/test_resource.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    35591 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/test_schema.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5021 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_search.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5671 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_stream.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2534 2021-12-27 14:46:55.000000 asdf-2.9.1/asdf/tests/test_tagged.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1513 2020-08-14 18:53:55.000000 asdf-2.9.1/asdf/tests/test_treeutil.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    19851 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/test_types.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3485 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/tests/test_util.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8642 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/test_versioning.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8314 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/tests/test_yaml.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    14975 2022-01-25 17:23:32.000000 asdf-2.9.1/asdf/treeutil.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    13329 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/type_index.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    16316 2021-12-27 14:46:55.000000 asdf-2.9.1/asdf/types.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    14794 2022-01-25 17:23:32.000000 asdf-2.9.1/asdf/util.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)       18 2022-02-03 15:48:05.000000 asdf-2.9.1/asdf/version.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5998 2021-07-30 18:34:36.000000 asdf-2.9.1/asdf/versioning.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    14604 2022-02-01 15:44:28.000000 asdf-2.9.1/asdf/yamlutil.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.330359 asdf-2.9.1/asdf-standard/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.361811 asdf-2.9.1/asdf-standard/reference_files/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.378893 asdf-2.9.1/asdf-standard/reference_files/1.0.0/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      452 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/ascii.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      337 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/ascii.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      504 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/basic.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      345 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/basic.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5737 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/complex.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    18513 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/complex.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1029 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/compressed.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1499 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/compressed.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      360 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/exploded.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      345 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/exploded.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      415 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/exploded0000.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1158 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/float.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1181 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/float.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2214 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/int.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1319 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/int.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      623 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/shared.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      425 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/shared.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      923 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/stream.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      690 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/stream.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      637 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/unicode_bmp.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      427 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/unicode_bmp.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      637 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/unicode_spp.asdf
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      443 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/1.0.0/unicode_spp.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      728 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/README.rst
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.380357 asdf-2.9.1/asdf-standard/reference_files/generate/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      245 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/generate/README.rst
--rwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)     4383 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/reference_files/generate/generate
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.329663 asdf-2.9.1/asdf-standard/resources/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.329789 asdf-2.9.1/asdf-standard/resources/asdf-format.org/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.330139 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.386191 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8041 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8706 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     9020 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     9665 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    10005 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.4.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8379 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.5.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8379 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.6.0.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.386933 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/schemas/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2854 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/schemas/extension_manifest-1.0.0.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.330493 asdf-2.9.1/asdf-standard/schemas/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.332281 asdf-2.9.1/asdf-standard/schemas/stsci.edu/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.392290 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2643 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/asdf-schema-1.0.0.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.402257 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1419 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/asdf-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1478 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/asdf-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1043 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/column-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2873 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/complex-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      301 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/constant-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      671 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/extension_metadata-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1018 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/externalarray-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      828 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/history_entry-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1627 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/integer-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    11708 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/ndarray-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      916 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/software-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      570 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/subclass_metadata-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2889 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/table-1.0.0.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.403051 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/fits/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3939 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/fits/fits-1.0.0.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.404485 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/time/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8303 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/time/time-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     7938 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/time/time-1.1.0.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.592740 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      780 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      780 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      780 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1240 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1240 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1326 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1326 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      655 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      625 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      687 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1380 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/airy_disk2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      935 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/blackbody-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1223 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1223 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1285 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1285 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1002 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/box1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1421 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/box2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1277 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/broken_power_law1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      474 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cobe_quad_spherical_cube-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      474 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cobe_quad_spherical_cube-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      474 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cobe_quad_spherical_cube-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1129 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1129 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1129 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1964 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1964 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1964 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1327 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1327 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1451 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1451 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      930 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      930 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      900 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      900 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      767 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      767 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      737 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      737 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1150 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1150 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1120 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1120 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      785 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      785 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      755 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      755 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      552 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      552 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      614 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      614 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      618 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.4.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      409 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      409 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      409 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      919 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      919 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      981 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      981 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1193 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1193 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1317 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1317 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1267 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/disk2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      872 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      872 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      872 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1054 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/domain-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1071 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/drude1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1853 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ellipse2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      814 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/exponential1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1233 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/exponential_cutoff_power_law1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1807 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/fix_inputs-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1807 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/fix_inputs-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1000 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gaussian1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2038 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gaussian2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      774 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      744 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      744 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      864 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      864 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      864 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      797 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      797 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      797 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      566 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      566 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      566 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      500 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/identity-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      500 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/identity-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      500 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/identity-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1163 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/king_projected_analytic1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4234 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4524 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4524 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      640 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/linear1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1215 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/log_parabola1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      837 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/logarithmic1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1040 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/lorentz1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      540 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/math_functions-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      717 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      717 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      717 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1197 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/moffat1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1400 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/moffat2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      910 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      910 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      910 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      886 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      886 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      886 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      725 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/multiplyscale-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1696 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ortho_polynomial-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      761 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      761 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      761 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      990 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/planar2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      666 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      666 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      666 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      868 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/plummer1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      419 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/polyconic-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      419 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/polyconic-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      419 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/polyconic-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1313 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1313 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1356 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      612 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      612 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      612 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      960 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/power_law1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      420 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/pseudoconic-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      420 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/pseudoconic-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      420 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/pseudoconic-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      617 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      617 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      617 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      459 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/quad_spherical_cube-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      459 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/quad_spherical_cube-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      459 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/quad_spherical_cube-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      679 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      679 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      679 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      652 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/redshift_scale_factor-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3135 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3105 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3105 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2085 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2143 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2143 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2265 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1060 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ricker_wavelet1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1239 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ricker_wavelet2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1480 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ring2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      549 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      549 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      611 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      611 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1464 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1464 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1650 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1650 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1315 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate_sequence_3d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      653 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      653 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      653 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      427 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/scale-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      427 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/scale-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      491 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/scale-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1147 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sersic1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1880 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sersic2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      435 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/shift-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      435 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/shift-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      497 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/shift-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      949 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sine1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      803 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      773 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      773 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1333 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1333 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1489 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1471 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/smoothly_broken_power_law1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      830 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      800 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      800 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      883 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      883 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      883 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1886 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1886 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1969 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      464 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/tangential_spherical_cube-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      464 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/tangential_spherical_cube-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      464 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/tangential_spherical_cube-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1032 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1032 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      825 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1285 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/trapezoid1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1595 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/trapezoid_disk2d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1271 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/voigt1d-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      701 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      701 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      701 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      918 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      888 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      888 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      758 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      728 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      728 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1427 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1427 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1551 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1551 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.3.0.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.594361 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/unit/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      829 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/unit/defunit-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1321 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/unit/quantity-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      559 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/unit/unit-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3176 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3216 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3268 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3356 2022-02-03 15:47:44.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.3.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3720 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.4.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4983 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.5.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      781 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.6.0.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.604158 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      512 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/celestial_frame-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      512 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/celestial_frame-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      532 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/composite_frame-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      509 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/composite_frame-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5756 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/frame-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5449 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/frame-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1042 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/icrs_coord-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      683 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/spectral_frame-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      683 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/spectral_frame-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      817 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      817 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      817 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.2.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1054 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.0.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1013 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.1.0.yaml
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1013 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.2.0.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.604905 asdf-2.9.1/asdf-standard/schemas/stsci.edu/yaml-schema/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4552 2022-02-02 17:14:51.000000 asdf-2.9.1/asdf-standard/schemas/stsci.edu/yaml-schema/draft-01.yaml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.607830 asdf-2.9.1/asdf.egg-info/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    11698 2022-02-03 15:48:05.000000 asdf-2.9.1/asdf.egg-info/PKG-INFO
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    25767 2022-02-03 15:48:06.000000 asdf-2.9.1/asdf.egg-info/SOURCES.txt
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        1 2022-02-03 15:48:05.000000 asdf-2.9.1/asdf.egg-info/dependency_links.txt
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      241 2022-02-03 15:48:05.000000 asdf-2.9.1/asdf.egg-info/entry_points.txt
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      324 2022-02-03 15:48:05.000000 asdf-2.9.1/asdf.egg-info/requires.txt
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)       17 2022-02-03 15:48:05.000000 asdf-2.9.1/asdf.egg-info/top_level.txt
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.674055 asdf-2.9.1/compatibility_tests/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      518 2020-08-14 18:53:55.000000 asdf-2.9.1/compatibility_tests/README.md
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      458 2020-08-14 18:53:55.000000 asdf-2.9.1/compatibility_tests/assert_file_correct.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      570 2021-07-30 18:34:36.000000 asdf-2.9.1/compatibility_tests/common.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      609 2021-04-01 18:15:20.000000 asdf-2.9.1/compatibility_tests/generate_file.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     7095 2022-02-01 15:44:28.000000 asdf-2.9.1/compatibility_tests/test_file_compatibility.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      430 2021-07-30 18:34:36.000000 asdf-2.9.1/conftest.py
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.337176 asdf-2.9.1/docker/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.675312 asdf-2.9.1/docker/s390x/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      850 2021-07-30 18:34:36.000000 asdf-2.9.1/docker/s390x/Dockerfile
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      399 2021-07-30 18:34:36.000000 asdf-2.9.1/docker/s390x/README.md
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.677922 asdf-2.9.1/docs/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4724 2019-11-26 21:28:29.000000 asdf-2.9.1/docs/Makefile
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.678554 asdf-2.9.1/docs/_static/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      145 2020-01-23 22:13:16.000000 asdf-2.9.1/docs/_static/custom.css
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.338439 asdf-2.9.1/docs/_templates/
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.680650 asdf-2.9.1/docs/_templates/autosummary/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      250 2019-11-26 21:28:29.000000 asdf-2.9.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      251 2019-11-26 21:28:29.000000 asdf-2.9.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      252 2019-11-26 21:28:29.000000 asdf-2.9.1/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.690943 asdf-2.9.1/docs/asdf/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     9188 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/arrays.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      949 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/asdf_tool.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    12625 2022-02-03 15:47:44.000000 asdf-2.9.1/docs/asdf/changes.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5366 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/config.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      395 2021-07-30 18:34:36.000000 asdf-2.9.1/docs/asdf/developer_api.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    38098 2021-07-30 18:34:36.000000 asdf-2.9.1/docs/asdf/developer_overview.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    10499 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/developer_versioning.rst
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.696985 asdf-2.9.1/docs/asdf/extending/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2884 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/extending/compressors.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    10746 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/extending/converters.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    12803 2022-02-01 15:44:28.000000 asdf-2.9.1/docs/asdf/extending/extensions.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    33177 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/extending/legacy.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     3608 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/extending/manifests.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8105 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/extending/resources.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8254 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/extending/schemas.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4768 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/extending/uris.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     8258 2022-02-01 15:44:28.000000 asdf-2.9.1/docs/asdf/extending/use_cases.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    24808 2022-02-01 15:44:28.000000 asdf-2.9.1/docs/asdf/features.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1680 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/install.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     1197 2021-07-30 18:34:36.000000 asdf-2.9.1/docs/asdf/overview.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)      209 2021-07-30 18:34:36.000000 asdf-2.9.1/docs/asdf/user_api.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     9164 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/asdf/using_extensions.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     5862 2022-01-25 17:23:32.000000 asdf-2.9.1/docs/conf.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2153 2022-02-01 15:44:28.000000 asdf-2.9.1/docs/index.rst
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4513 2019-11-26 21:28:29.000000 asdf-2.9.1/docs/make.bat
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.697883 asdf-2.9.1/docs/sphinxext/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2021-07-30 18:34:36.000000 asdf-2.9.1/docs/sphinxext/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     4749 2021-07-30 18:34:36.000000 asdf-2.9.1/docs/sphinxext/example.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)       76 2021-05-12 20:18:35.000000 asdf-2.9.1/pyproject.toml
-drwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)        0 2022-02-03 15:48:06.698505 asdf-2.9.1/pytest_asdf/
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)        0 2021-07-30 18:34:36.000000 asdf-2.9.1/pytest_asdf/__init__.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)    11665 2021-07-30 18:34:36.000000 asdf-2.9.1/pytest_asdf/plugin.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2964 2022-02-03 15:48:06.700168 asdf-2.9.1/setup.cfg
--rwxr-xr-x   0 eslavich  (2356) STSCI\science  (1031)     1173 2022-02-01 15:44:29.000000 asdf-2.9.1/setup.py
--rw-r--r--   0 eslavich  (2356) STSCI\science  (1031)     2772 2022-02-01 15:44:28.000000 asdf-2.9.1/tox.ini
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.985379 asdf-2.9.2/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.783856 asdf-2.9.2/.github/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.799008 asdf-2.9.2/.github/workflows/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      541 2022-01-28 22:12:47.000000 asdf-2.9.2/.github/workflows/changelog.yml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4063 2022-02-07 20:41:31.000000 asdf-2.9.2/.github/workflows/ci.yml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3444 2022-02-07 20:41:31.000000 asdf-2.9.2/.github/workflows/downstream.yml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      694 2022-02-08 00:49:36.000000 asdf-2.9.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1174 2022-02-07 20:31:22.000000 asdf-2.9.2/.github/workflows/s390x.yml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    23252 2022-02-07 20:49:38.000000 asdf-2.9.2/CHANGES.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3246 2022-01-28 22:12:47.000000 asdf-2.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1035 2022-01-28 22:12:47.000000 asdf-2.9.2/CONTRIBUTING.md
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1539 2022-01-28 22:12:47.000000 asdf-2.9.2/LICENSE
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)       92 2022-01-28 22:12:47.000000 asdf-2.9.2/MANIFEST.in
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    11698 2022-02-08 01:08:56.985636 asdf-2.9.2/PKG-INFO
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    10762 2022-02-07 20:31:22.000000 asdf-2.9.2/README.rst
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.814120 asdf-2.9.2/asdf/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      740 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2025 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/_convenience.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    11445 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/_display.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      576 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/_helpers.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    66125 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/asdf.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      523 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/asdftypes.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    47971 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/block.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.925552 asdf-2.9.2/asdf/commands/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      592 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1966 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/defragment.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    12116 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/diff.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    11646 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/edit.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3321 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/exploded.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2638 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/extension.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1595 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/extract.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1278 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/info.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1967 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/main.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1364 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/remove_hdu.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1606 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tags.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.929506 asdf-2.9.2/asdf/commands/tests/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/__init__.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.934487 asdf-2.9.2/asdf/commands/tests/data/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    80469 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/block0.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    80469 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/block1.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      276 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/blocks.diff
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1246 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/frames.diff
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4191 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/frames0.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3793 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/frames1.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1160 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/frames_ignore_asdf_library.diff
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/frames_ignore_both.diff
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      103 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/frames_ignore_reference_frame.diff
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      269 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/frames_minimal.diff
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)       41 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/simple_inline_array.diff
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      495 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/simple_inline_array0.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      495 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/data/simple_inline_array1.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1367 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tests/test_defragment.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2320 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tests/test_diff.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     9360 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tests/test_edit.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1592 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tests/test_exploded.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      454 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/test_extension.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      984 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tests/test_extract.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1042 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tests/test_info.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      415 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tests/test_main.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      927 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tests/test_remove_hdu.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      598 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/commands/tests/test_tags.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      874 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/tests/test_to_yaml.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1936 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/commands/to_yaml.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.934958 asdf-2.9.2/asdf/compat/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/compat/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      176 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/compat/numpycompat.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    10430 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/compression.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    12169 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/config.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1276 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/conftest.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      649 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/constants.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2376 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/entry_points.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      528 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/exceptions.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.937659 asdf-2.9.2/asdf/extension/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      947 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/extension/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2543 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/extension/_compressor.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    11052 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/extension/_converter.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    10835 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/extension/_extension.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8031 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/extension/_legacy.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     6170 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/extension/_manager.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3510 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/extension/_manifest.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2571 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/extension/_tag.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.939315 asdf-2.9.2/asdf/extern/
+-rwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)     7095 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/extern/RangeHTTPServer.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        8 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/extern/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4170 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/extern/atomicfile.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    12069 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/fits_embed.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    33320 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/generic_io.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5317 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/reference.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5854 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/resolver.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     9003 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/resource.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    26685 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/schema.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    12515 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/search.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1788 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/stream.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4269 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tagged.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.939675 asdf-2.9.2/asdf/tags/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tags/__init__.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.942474 asdf-2.9.2/asdf/tags/core/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1641 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      531 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/complex.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      434 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/constant.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2185 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/external_reference.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3438 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/integer.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    25272 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/ndarray.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.945083 asdf-2.9.2/asdf/tags/core/tests/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tags/core/tests/__init__.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.946475 asdf-2.9.2/asdf/tags/core/tests/data/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tags/core/tests/data/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      473 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tags/core/tests/data/datatype-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      187 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tags/core/tests/data/ndim-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1365 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/tests/test_complex.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      636 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/tests/test_extension_metadata.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      340 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/tests/test_external_reference.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8452 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/tests/test_history.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2317 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/tests/test_integer.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    25698 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tags/core/tests/test_ndarray.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.947225 asdf-2.9.2/asdf/testing/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-03 19:00:01.000000 asdf-2.9.2/asdf/testing/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1555 2022-02-03 19:00:01.000000 asdf-2.9.2/asdf/testing/helpers.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.960342 asdf-2.9.2/asdf/tests/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1764 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      736 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/conftest.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      608 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/coveragerc
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.967614 asdf-2.9.2/asdf/tests/data/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3840 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/data/asdf.fits.gz
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      138 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/complex-42.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      149 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/custom-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      214 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/custom_flow-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      215 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/custom_flow-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      545 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/custom_schema.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      306 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/custom_schema_definitions.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      395 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/custom_schema_external_ref.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      158 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/custom_style-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1072 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/default-1.0.0.yaml
+-rwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)     2203 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/example_schema.json
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8641 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/data/extension_check.fits
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      525 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/foreign_tag_reference-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      581 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/fraction-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      442 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/fraction_with_inverse-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      355 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/fractional_2d_coord-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      137 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/missing-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      407 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/one_of-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      183 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/self_referencing-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      378 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/tag_reference-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5760 2022-01-28 22:12:47.000000 asdf-2.9.2/asdf/tests/data/version_mismatch.fits
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    15287 2022-02-07 20:40:58.000000 asdf-2.9.2/asdf/tests/helpers.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2070 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/httpserver.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    18332 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_api.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    24895 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_array_blocks.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    11537 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_asdf.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     7123 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_compression.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    12398 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_config.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4844 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_entry_points.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    24805 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_extension.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5348 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_file_format.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    17630 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_fits_embed.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    24158 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_generic_io.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1153 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_helpers.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3438 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_integration.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8301 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_reference.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2484 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_reference_files.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3647 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_resolver.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    12114 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_resource.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    35591 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_schema.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5021 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_search.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5671 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_stream.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2534 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_tagged.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1513 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_treeutil.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    19854 2022-02-07 20:40:58.000000 asdf-2.9.2/asdf/tests/test_types.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3485 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/tests/test_util.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8642 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_versioning.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8314 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/tests/test_yaml.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    14975 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/treeutil.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    13329 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/type_index.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    16316 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/types.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    14784 2022-02-07 20:42:39.000000 asdf-2.9.2/asdf/util.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)       18 2022-02-08 01:08:54.000000 asdf-2.9.2/asdf/version.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5998 2022-01-31 19:30:31.000000 asdf-2.9.2/asdf/versioning.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    14604 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf/yamlutil.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.785295 asdf-2.9.2/asdf-standard/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.814557 asdf-2.9.2/asdf-standard/reference_files/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.822558 asdf-2.9.2/asdf-standard/reference_files/1.0.0/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      452 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/ascii.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      337 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/ascii.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      504 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/basic.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      345 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/basic.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5737 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/complex.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    18513 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/complex.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1029 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/compressed.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1499 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/compressed.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      360 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/exploded.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      345 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/exploded.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      415 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/exploded0000.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1158 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/float.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1181 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/float.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2214 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/int.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1319 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/int.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      623 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/shared.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      425 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/shared.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      923 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/stream.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      690 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/stream.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      637 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/unicode_bmp.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      427 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/unicode_bmp.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      637 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/unicode_spp.asdf
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      443 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/1.0.0/unicode_spp.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      728 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/README.rst
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.823229 asdf-2.9.2/asdf-standard/reference_files/generate/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      245 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/generate/README.rst
+-rwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)     4383 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/reference_files/generate/generate
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.784819 asdf-2.9.2/asdf-standard/resources/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.784917 asdf-2.9.2/asdf-standard/resources/asdf-format.org/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.785148 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.825514 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8041 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8706 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     9020 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     9665 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    10005 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.4.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8379 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.5.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8379 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.6.0.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.825831 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/schemas/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2854 2022-02-07 20:31:22.000000 asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/schemas/extension_manifest-1.0.0.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.785487 asdf-2.9.2/asdf-standard/schemas/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.787534 asdf-2.9.2/asdf-standard/schemas/stsci.edu/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.828701 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2643 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/asdf-schema-1.0.0.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.832708 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1419 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/asdf-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1478 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/asdf-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1043 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/column-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2873 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/complex-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      301 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/constant-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      671 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/extension_metadata-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1018 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/externalarray-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      828 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/history_entry-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1627 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/integer-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    11708 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/ndarray-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      916 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/software-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      570 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/subclass_metadata-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2889 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/table-1.0.0.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.832986 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/fits/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3939 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/fits/fits-1.0.0.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.833553 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/time/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8303 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/time/time-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     7938 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/time/time-1.1.0.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.913148 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      780 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      780 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      780 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1240 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1240 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1326 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1326 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      655 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      625 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      687 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1380 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/airy_disk2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      935 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/blackbody-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1223 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1223 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1285 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1285 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1002 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/box1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1421 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/box2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1277 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/broken_power_law1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      474 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cobe_quad_spherical_cube-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      474 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cobe_quad_spherical_cube-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      474 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cobe_quad_spherical_cube-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1129 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1129 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1129 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1964 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1964 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1964 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1327 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1327 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1451 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1451 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      930 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      930 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      900 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      900 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      767 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      767 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      737 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      737 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1150 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1150 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1120 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1120 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      785 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      785 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      755 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      755 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      552 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      552 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      614 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      614 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      618 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.4.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      409 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      409 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      409 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      919 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      919 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      981 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      981 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1193 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1193 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1317 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1317 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1267 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/disk2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      872 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      872 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      872 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1054 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/domain-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1071 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/drude1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1853 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ellipse2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      814 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/exponential1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1233 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/exponential_cutoff_power_law1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1807 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/fix_inputs-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1807 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/fix_inputs-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1000 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gaussian1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2038 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gaussian2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      774 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      744 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      744 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      864 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      864 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      864 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      797 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      797 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      797 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      566 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      566 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      566 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      500 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/identity-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      500 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/identity-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      500 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/identity-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1163 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/king_projected_analytic1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4234 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4524 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4524 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      640 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/linear1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1215 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/log_parabola1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      837 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/logarithmic1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1040 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/lorentz1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      540 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/math_functions-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      717 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      717 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      717 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1197 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/moffat1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1400 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/moffat2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      910 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      910 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      910 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      886 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      886 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      886 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      725 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/multiplyscale-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1696 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ortho_polynomial-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      761 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      761 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      761 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      990 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/planar2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      666 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      666 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      666 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      868 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/plummer1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      419 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/polyconic-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      419 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/polyconic-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      419 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/polyconic-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1313 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1313 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1356 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      612 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      612 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      612 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      960 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/power_law1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      420 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/pseudoconic-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      420 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/pseudoconic-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      420 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/pseudoconic-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      617 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      617 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      617 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      459 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/quad_spherical_cube-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      459 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/quad_spherical_cube-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      459 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/quad_spherical_cube-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      679 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      679 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      679 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      652 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/redshift_scale_factor-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3135 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3105 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3105 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2085 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2143 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2143 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2265 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1060 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ricker_wavelet1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1239 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ricker_wavelet2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1480 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ring2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      549 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      549 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      611 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      611 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1464 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1464 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1650 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1650 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1315 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate_sequence_3d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      653 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      653 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      653 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      427 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/scale-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      427 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/scale-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      491 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/scale-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1147 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sersic1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1880 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sersic2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      435 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/shift-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      435 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/shift-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      497 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/shift-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      949 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sine1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      803 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      773 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      773 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1333 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1333 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1489 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1471 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/smoothly_broken_power_law1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      830 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      800 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      800 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      883 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      883 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      883 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1886 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1886 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1969 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      464 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/tangential_spherical_cube-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      464 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/tangential_spherical_cube-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      464 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/tangential_spherical_cube-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1032 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1032 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      825 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1285 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/trapezoid1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1595 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/trapezoid_disk2d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1271 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/voigt1d-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      701 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      701 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      701 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      918 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      888 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      888 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      758 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      728 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      728 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1427 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1427 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1551 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1551 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.3.0.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.914242 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/unit/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      829 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/unit/defunit-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1321 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/unit/quantity-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      559 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/unit/unit-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3176 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3216 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3268 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3356 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.3.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3720 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.4.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4983 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.5.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      781 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.6.0.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.919509 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      512 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/celestial_frame-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      512 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/celestial_frame-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      532 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/composite_frame-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      509 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/composite_frame-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5756 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/frame-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5449 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/frame-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1042 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/icrs_coord-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      683 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/spectral_frame-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      683 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/spectral_frame-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      817 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      817 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      817 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.2.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1054 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.0.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1013 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.1.0.yaml
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1013 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.2.0.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.919873 asdf-2.9.2/asdf-standard/schemas/stsci.edu/yaml-schema/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4552 2022-02-04 16:49:28.000000 asdf-2.9.2/asdf-standard/schemas/stsci.edu/yaml-schema/draft-01.yaml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.921728 asdf-2.9.2/asdf.egg-info/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    11698 2022-02-08 01:08:54.000000 asdf-2.9.2/asdf.egg-info/PKG-INFO
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    25805 2022-02-08 01:08:55.000000 asdf-2.9.2/asdf.egg-info/SOURCES.txt
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        1 2022-02-08 01:08:54.000000 asdf-2.9.2/asdf.egg-info/dependency_links.txt
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      241 2022-02-08 01:08:54.000000 asdf-2.9.2/asdf.egg-info/entry_points.txt
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      324 2022-02-08 01:08:54.000000 asdf-2.9.2/asdf.egg-info/requires.txt
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)       17 2022-02-08 01:08:54.000000 asdf-2.9.2/asdf.egg-info/top_level.txt
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.969278 asdf-2.9.2/compatibility_tests/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      518 2022-01-28 22:12:47.000000 asdf-2.9.2/compatibility_tests/README.md
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      458 2022-01-28 22:12:47.000000 asdf-2.9.2/compatibility_tests/assert_file_correct.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      570 2022-01-28 22:12:47.000000 asdf-2.9.2/compatibility_tests/common.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      609 2022-01-28 22:12:47.000000 asdf-2.9.2/compatibility_tests/generate_file.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     7077 2022-02-07 20:42:39.000000 asdf-2.9.2/compatibility_tests/test_file_compatibility.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      430 2022-01-28 22:12:47.000000 asdf-2.9.2/conftest.py
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.791134 asdf-2.9.2/docker/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.970077 asdf-2.9.2/docker/s390x/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      850 2022-01-28 22:12:47.000000 asdf-2.9.2/docker/s390x/Dockerfile
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      399 2022-01-28 22:12:47.000000 asdf-2.9.2/docker/s390x/README.md
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.972327 asdf-2.9.2/docs/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4724 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/Makefile
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.972963 asdf-2.9.2/docs/_static/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      145 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/_static/custom.css
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.792267 asdf-2.9.2/docs/_templates/
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.974118 asdf-2.9.2/docs/_templates/autosummary/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      250 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      251 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      252 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.980241 asdf-2.9.2/docs/asdf/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     9188 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/arrays.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      949 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/asdf_tool.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    12881 2022-02-07 20:49:38.000000 asdf-2.9.2/docs/asdf/changes.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5366 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/config.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      395 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/developer_api.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    38098 2022-02-07 20:31:22.000000 asdf-2.9.2/docs/asdf/developer_overview.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    10499 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/developer_versioning.rst
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.983686 asdf-2.9.2/docs/asdf/extending/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2884 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/extending/compressors.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    10746 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/extending/converters.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    12803 2022-02-07 20:31:22.000000 asdf-2.9.2/docs/asdf/extending/extensions.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    33177 2022-02-07 20:31:22.000000 asdf-2.9.2/docs/asdf/extending/legacy.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3608 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/extending/manifests.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8105 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/extending/resources.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8254 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/extending/schemas.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4768 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/extending/uris.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     8258 2022-02-07 20:31:22.000000 asdf-2.9.2/docs/asdf/extending/use_cases.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    24808 2022-02-07 20:31:22.000000 asdf-2.9.2/docs/asdf/features.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1680 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/install.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     1197 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/overview.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)      209 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/asdf/user_api.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     9164 2022-02-07 20:31:22.000000 asdf-2.9.2/docs/asdf/using_extensions.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     5862 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/conf.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2153 2022-02-07 20:31:22.000000 asdf-2.9.2/docs/index.rst
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4513 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/make.bat
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.984228 asdf-2.9.2/docs/sphinxext/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/docs/sphinxext/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     4749 2022-02-07 20:31:22.000000 asdf-2.9.2/docs/sphinxext/example.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)       76 2022-01-28 22:12:47.000000 asdf-2.9.2/pyproject.toml
+drwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-02-08 01:08:56.984757 asdf-2.9.2/pytest_asdf/
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)        0 2022-01-28 22:12:47.000000 asdf-2.9.2/pytest_asdf/__init__.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)    10199 2022-02-07 20:42:02.000000 asdf-2.9.2/pytest_asdf/plugin.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     2964 2022-02-08 01:08:56.986688 asdf-2.9.2/setup.cfg
+-rwxr-xr-x   0 wjamieson  (2813) STSCI\science  (1031)     1291 2022-02-07 20:40:46.000000 asdf-2.9.2/setup.py
+-rw-r--r--   0 wjamieson  (2813) STSCI\science  (1031)     3089 2022-02-07 20:41:31.000000 asdf-2.9.2/tox.ini
```

### Comparing `asdf-2.9.1/.github/workflows/changelog.yml` & `asdf-2.9.2/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/.github/workflows/ci.yml` & `asdf-2.9.2/.github/workflows/ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -77,26 +77,46 @@
             os: ubuntu-latest
             python-version: "3.9"
             toxenv: checkdocs
 
           - name: Astropy Dev
             os: ubuntu-latest
             python-version: "3.9"
-            toxenv: py38-astropydev
+            toxenv: py39-astropydev
+
+          - name: ASDF-Astropy Dev
+            os: ubuntu-latest
+            python-version: "3.9"
+            toxenv: py39-asdfastropydev
 
           - name: GWCS Dev
             os: ubuntu-latest
             python-version: "3.9"
-            toxenv: py38-gwcsdev
+            toxenv: py39-gwcsdev
 
           # Fail
           - name: Numpy Dev
             os: ubuntu-latest
             python-version: "3.9"
-            toxenv: py38-numpydev
+            toxenv: py39-numpydev
+
+          - name: ASDF-Transform-Schemas Dev
+            os: ubuntu-latest
+            python-version: "3.9"
+            toxenv: py39-asdftransformschemasdev
+
+          - name: ASDF-WCS-Schemas Dev
+            os: ubuntu-latest
+            python-version: "3.9"
+            toxenv: py39-asdfwcsschemasdev
+
+          - name: ASDF-Coordinates-Schemas Dev
+            os: ubuntu-latest
+            python-version: "3.9"
+            toxenv: py39-asdfcoordinatesschemasdev
 
           # Fail
           - name: Pre-Release Dependencies
             os: ubuntu-latest
             python-version: "3.9"
             toxenv: prerelease
```

### Comparing `asdf-2.9.1/.github/workflows/s390x.yml` & `asdf-2.9.2/.github/workflows/s390x.yml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/CHANGES.rst` & `asdf-2.9.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2.9.2 (2022-02-07)
+------------------
+
+- Fix deprecation warnings stemming from the release of pytest 7.0.0. [#1075]
+
+- Fix bug in pytest plugin when schemas are not in a directory named "schemas". [#1076]
+
 2.9.1 (2022-02-03)
 ------------------
 
 - Fix typo in testing module ``__init__.py`` name. [#1071]
 
 2.9.0 (2022-02-02)
 ------------------
```

### Comparing `asdf-2.9.1/CODE_OF_CONDUCT.md` & `asdf-2.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/CONTRIBUTING.md` & `asdf-2.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/LICENSE` & `asdf-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/PKG-INFO` & `asdf-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdf
-Version: 2.9.1
+Version: 2.9.2
 Summary: Python implementation of the ASDF Standard
 Home-page: http://github.com/asdf-format/asdf
 Author: The ASDF Developers
 Author-email: help@stsci.edu
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/asdf-format/asdf/issues
 Project-URL: Documentation, https://asdf.readthedocs.io/en/stable
```

### Comparing `asdf-2.9.1/README.rst` & `asdf-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/__init__.py` & `asdf-2.9.2/asdf/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/_convenience.py` & `asdf-2.9.2/asdf/_convenience.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/_display.py` & `asdf-2.9.2/asdf/_display.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/_helpers.py` & `asdf-2.9.2/asdf/_helpers.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/asdf.py` & `asdf-2.9.2/asdf/asdf.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/asdftypes.py` & `asdf-2.9.2/asdf/asdftypes.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/block.py` & `asdf-2.9.2/asdf/block.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/__init__.py` & `asdf-2.9.2/asdf/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/defragment.py` & `asdf-2.9.2/asdf/commands/defragment.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/diff.py` & `asdf-2.9.2/asdf/commands/diff.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/edit.py` & `asdf-2.9.2/asdf/commands/edit.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/exploded.py` & `asdf-2.9.2/asdf/commands/exploded.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/extension.py` & `asdf-2.9.2/asdf/commands/extension.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/extract.py` & `asdf-2.9.2/asdf/commands/extract.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/info.py` & `asdf-2.9.2/asdf/commands/info.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/main.py` & `asdf-2.9.2/asdf/commands/main.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/remove_hdu.py` & `asdf-2.9.2/asdf/commands/remove_hdu.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tags.py` & `asdf-2.9.2/asdf/commands/tags.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/data/block0.asdf` & `asdf-2.9.2/asdf/commands/tests/data/block0.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/data/block1.asdf` & `asdf-2.9.2/asdf/commands/tests/data/block1.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/data/frames.diff` & `asdf-2.9.2/asdf/commands/tests/data/frames.diff`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/data/frames0.asdf` & `asdf-2.9.2/asdf/commands/tests/data/frames0.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/data/frames1.asdf` & `asdf-2.9.2/asdf/commands/tests/data/frames1.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/data/frames_ignore_asdf_library.diff` & `asdf-2.9.2/asdf/commands/tests/data/frames_ignore_asdf_library.diff`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/test_defragment.py` & `asdf-2.9.2/asdf/commands/tests/test_defragment.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/test_diff.py` & `asdf-2.9.2/asdf/commands/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/test_edit.py` & `asdf-2.9.2/asdf/commands/tests/test_edit.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/test_exploded.py` & `asdf-2.9.2/asdf/commands/tests/test_exploded.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/test_extract.py` & `asdf-2.9.2/asdf/commands/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/test_info.py` & `asdf-2.9.2/asdf/commands/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/test_remove_hdu.py` & `asdf-2.9.2/asdf/commands/tests/test_remove_hdu.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/test_tags.py` & `asdf-2.9.2/asdf/commands/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/tests/test_to_yaml.py` & `asdf-2.9.2/asdf/commands/tests/test_to_yaml.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/commands/to_yaml.py` & `asdf-2.9.2/asdf/commands/to_yaml.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/compression.py` & `asdf-2.9.2/asdf/compression.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/config.py` & `asdf-2.9.2/asdf/config.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/conftest.py` & `asdf-2.9.2/asdf/conftest.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/constants.py` & `asdf-2.9.2/asdf/constants.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/entry_points.py` & `asdf-2.9.2/asdf/entry_points.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/exceptions.py` & `asdf-2.9.2/asdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extension/__init__.py` & `asdf-2.9.2/asdf/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extension/_compressor.py` & `asdf-2.9.2/asdf/extension/_compressor.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extension/_converter.py` & `asdf-2.9.2/asdf/extension/_converter.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extension/_extension.py` & `asdf-2.9.2/asdf/extension/_extension.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extension/_legacy.py` & `asdf-2.9.2/asdf/extension/_legacy.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extension/_manager.py` & `asdf-2.9.2/asdf/extension/_manager.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extension/_manifest.py` & `asdf-2.9.2/asdf/extension/_manifest.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extension/_tag.py` & `asdf-2.9.2/asdf/extension/_tag.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extern/RangeHTTPServer.py` & `asdf-2.9.2/asdf/extern/RangeHTTPServer.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/extern/atomicfile.py` & `asdf-2.9.2/asdf/extern/atomicfile.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/fits_embed.py` & `asdf-2.9.2/asdf/fits_embed.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/generic_io.py` & `asdf-2.9.2/asdf/generic_io.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/reference.py` & `asdf-2.9.2/asdf/reference.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/resolver.py` & `asdf-2.9.2/asdf/resolver.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/resource.py` & `asdf-2.9.2/asdf/resource.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/schema.py` & `asdf-2.9.2/asdf/schema.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/search.py` & `asdf-2.9.2/asdf/search.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/stream.py` & `asdf-2.9.2/asdf/stream.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tagged.py` & `asdf-2.9.2/asdf/tagged.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/__init__.py` & `asdf-2.9.2/asdf/tags/core/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/complex.py` & `asdf-2.9.2/asdf/tags/core/complex.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/external_reference.py` & `asdf-2.9.2/asdf/tags/core/external_reference.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/integer.py` & `asdf-2.9.2/asdf/tags/core/integer.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/ndarray.py` & `asdf-2.9.2/asdf/tags/core/ndarray.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/tests/test_complex.py` & `asdf-2.9.2/asdf/tags/core/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/tests/test_extension_metadata.py` & `asdf-2.9.2/asdf/tags/core/tests/test_extension_metadata.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/tests/test_history.py` & `asdf-2.9.2/asdf/tags/core/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/tests/test_integer.py` & `asdf-2.9.2/asdf/tags/core/tests/test_integer.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tags/core/tests/test_ndarray.py` & `asdf-2.9.2/asdf/tags/core/tests/test_ndarray.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/testing/helpers.py` & `asdf-2.9.2/asdf/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/__init__.py` & `asdf-2.9.2/asdf/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/conftest.py` & `asdf-2.9.2/asdf/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/coveragerc` & `asdf-2.9.2/asdf/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/data/asdf.fits.gz` & `asdf-2.9.2/asdf/tests/data/asdf.fits.gz`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/data/custom_schema.yaml` & `asdf-2.9.2/asdf/tests/data/custom_schema.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/data/default-1.0.0.yaml` & `asdf-2.9.2/asdf/tests/data/default-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/data/example_schema.json` & `asdf-2.9.2/asdf/tests/data/example_schema.json`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/data/extension_check.fits` & `asdf-2.9.2/asdf/tests/data/extension_check.fits`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/data/foreign_tag_reference-1.0.0.yaml` & `asdf-2.9.2/asdf/tests/data/foreign_tag_reference-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/data/fraction-1.0.0.yaml` & `asdf-2.9.2/asdf/tests/data/fraction-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/data/version_mismatch.fits` & `asdf-2.9.2/asdf/tests/data/version_mismatch.fits`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/helpers.py` & `asdf-2.9.2/asdf/tests/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,22 +366,26 @@
     Parameters
     ----------
     warning_class : type, optional
         Assert only that no warnings of the specified class were
         emitted.
     """
     import pytest
-    with pytest.warns(None) as recorded_warnings:
-        yield
 
-    if warning_class is not None:
+    if warning_class is None:
+        with warnings.catch_warnings():
+            warnings.simplefilter("error")
+
+            yield
+    else:
+        with pytest.warns(Warning) as recorded_warnings:
+            yield
+
         assert not any(isinstance(w.message, warning_class) for w in recorded_warnings), \
             display_warnings(recorded_warnings)
-    else:
-        assert len(recorded_warnings) == 0, display_warnings(recorded_warnings)
 
 
 def assert_extension_correctness(extension):
     """
     Assert that an ASDF extension's types are all correctly formed and
     that the extension provides all of the required schemas.
```

### Comparing `asdf-2.9.1/asdf/tests/httpserver.py` & `asdf-2.9.2/asdf/tests/httpserver.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_api.py` & `asdf-2.9.2/asdf/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_array_blocks.py` & `asdf-2.9.2/asdf/tests/test_array_blocks.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_asdf.py` & `asdf-2.9.2/asdf/tests/test_asdf.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_compression.py` & `asdf-2.9.2/asdf/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_config.py` & `asdf-2.9.2/asdf/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_entry_points.py` & `asdf-2.9.2/asdf/tests/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_extension.py` & `asdf-2.9.2/asdf/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_file_format.py` & `asdf-2.9.2/asdf/tests/test_file_format.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_fits_embed.py` & `asdf-2.9.2/asdf/tests/test_fits_embed.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_generic_io.py` & `asdf-2.9.2/asdf/tests/test_generic_io.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_helpers.py` & `asdf-2.9.2/asdf/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_integration.py` & `asdf-2.9.2/asdf/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_reference.py` & `asdf-2.9.2/asdf/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_reference_files.py` & `asdf-2.9.2/asdf/tests/test_reference_files.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_resolver.py` & `asdf-2.9.2/asdf/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_resource.py` & `asdf-2.9.2/asdf/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_schema.py` & `asdf-2.9.2/asdf/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_search.py` & `asdf-2.9.2/asdf/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_stream.py` & `asdf-2.9.2/asdf/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_tagged.py` & `asdf-2.9.2/asdf/tests/test_tagged.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_treeutil.py` & `asdf-2.9.2/asdf/tests/test_treeutil.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_types.py` & `asdf-2.9.2/asdf/tests/test_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,15 @@
     - !core/ndarray-1.0.0
       [[1, 2, 3], [4, 5, 6]]
     - !<tag:nowhere.org:custom/also_undefined-1.3.0>
         - !core/ndarray-1.0.0 [[7],[8],[9],[10]]
         - !core/complex-1.0.0 3.14j
 """
     buff = helpers.yaml_to_asdf(yaml)
-    with pytest.warns(None) as warning:
+    with pytest.warns(Warning) as warning:
         afile = asdf.open(buff)
         missing = afile.tree['undefined_data']
 
     assert missing[0] == 5
     assert missing[1] == {'message': 'there is no tag'}
     assert (missing[2] == array([[1, 2, 3], [4, 5, 6]])).all()
     assert (missing[3][0] == array([[7],[8],[9],[10]])).all()
```

### Comparing `asdf-2.9.1/asdf/tests/test_util.py` & `asdf-2.9.2/asdf/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_versioning.py` & `asdf-2.9.2/asdf/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/tests/test_yaml.py` & `asdf-2.9.2/asdf/tests/test_yaml.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/treeutil.py` & `asdf-2.9.2/asdf/treeutil.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/type_index.py` & `asdf-2.9.2/asdf/type_index.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/types.py` & `asdf-2.9.2/asdf/types.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/util.py` & `asdf-2.9.2/asdf/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
 def minversion(module, version, inclusive=True, version_path='__version__'):
     """
     Returns `True` if the specified Python module satisfies a minimum version
     requirement, and `False` if not.
 
     By default this uses `pkg_resources.parse_version` to do the version
     comparison if available.  Otherwise it falls back on
-    `distutils.version.LooseVersion`.
+    `packaging.version.Version`.
 
     Parameters
     ----------
 
     module : module or `str`
         An imported module of which to check the version, or the name of
         that module (in which case an import of that module is attempted--
@@ -362,15 +362,15 @@
         have_version = getattr(module, version_path)
     else:
         have_version = resolve_name('.'.join([module.__name__, version_path]))
 
     try:
         from pkg_resources import parse_version
     except ImportError:
-        from distutils.version import LooseVersion as parse_version
+        from packaging.version import Version as parse_version
 
     if inclusive:
         return parse_version(have_version) >= parse_version(version)
     else:
         return parse_version(have_version) > parse_version(version)
```

### Comparing `asdf-2.9.1/asdf/versioning.py` & `asdf-2.9.2/asdf/versioning.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf/yamlutil.py` & `asdf-2.9.2/asdf/yamlutil.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/complex.asdf` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/complex.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/complex.yaml` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/complex.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/compressed.asdf` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/compressed.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/compressed.yaml` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/compressed.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/float.asdf` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/float.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/float.yaml` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/float.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/int.asdf` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/int.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/int.yaml` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/int.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/shared.asdf` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/shared.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/stream.asdf` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/stream.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/stream.yaml` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/stream.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/unicode_bmp.asdf` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/unicode_bmp.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/1.0.0/unicode_spp.asdf` & `asdf-2.9.2/asdf-standard/reference_files/1.0.0/unicode_spp.asdf`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/README.rst` & `asdf-2.9.2/asdf-standard/reference_files/README.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/reference_files/generate/generate` & `asdf-2.9.2/asdf-standard/reference_files/generate/generate`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.4.0.yaml` & `asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.4.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.5.0.yaml` & `asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.5.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/manifests/core-1.6.0.yaml` & `asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/manifests/core-1.6.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/resources/asdf-format.org/core/schemas/extension_manifest-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/resources/asdf-format.org/core/schemas/extension_manifest-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/asdf-schema-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/asdf-schema-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/asdf-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/asdf-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/asdf-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/asdf-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/column-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/column-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/complex-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/complex-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/extension_metadata-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/extension_metadata-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/externalarray-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/externalarray-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/history_entry-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/history_entry-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/integer-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/integer-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/ndarray-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/ndarray-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/software-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/software-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/subclass_metadata-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/subclass_metadata-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/core/table-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/core/table-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/fits/fits-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/fits/fits-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/time/time-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/time/time-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/time/time-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/time/time-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/add-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/affine-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/airy-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/airy_disk2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/airy_disk2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/blackbody-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/blackbody-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/bonne_equal_area-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/box1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/box1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/box2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/box2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/broken_power_law1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/broken_power_law1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/compose-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/concatenate-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equal_area-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_equidistant-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_orthomorphic-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/conic_perspective-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.4.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/constant-1.4.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_equal_area-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/cylindrical_perspective-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/disk2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/disk2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/divide-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/domain-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/domain-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/drude1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/drude1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ellipse2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ellipse2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/exponential1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/exponential1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/exponential_cutoff_power_law1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/exponential_cutoff_power_law1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/fix_inputs-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/fix_inputs-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/fix_inputs-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/fix_inputs-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gaussian1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gaussian1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gaussian2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gaussian2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/gnomonic-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/hammer_aitoff-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/healpix_polar-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/king_projected_analytic1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/king_projected_analytic1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/label_mapper-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/linear1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/linear1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/log_parabola1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/log_parabola1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/logarithmic1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/logarithmic1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/lorentz1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/lorentz1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/math_functions-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/math_functions-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/mercator-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/moffat1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/moffat1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/moffat2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/moffat2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/molleweide-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/multiply-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/multiplyscale-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/multiplyscale-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ortho_polynomial-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ortho_polynomial-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/parabolic-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/planar2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/planar2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/plate_carree-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/plummer1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/plummer1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/polynomial-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/power-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/power_law1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/power_law1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/pseudocylindrical-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/quadcube-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/redshift_scale_factor-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/redshift_scale_factor-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/regions_selector-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/remap_axes-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ricker_wavelet1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ricker_wavelet1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ricker_wavelet2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ricker_wavelet2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/ring2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/ring2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate2d-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate3d-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/rotate_sequence_3d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/rotate_sequence_3d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sanson_flamsteed-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sersic1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sersic1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sersic2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sersic2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/sine1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/sine1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_orthographic-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/slant_zenithal_perspective-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/smoothly_broken_power_law1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/smoothly_broken_power_law1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/stereographic-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/subtract-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/tabular-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/transform-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/trapezoid1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/trapezoid1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/trapezoid_disk2d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/trapezoid_disk2d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/voigt1d-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/voigt1d-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equal_area-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_equidistant-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/transform/zenithal_perspective-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/unit/defunit-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/unit/defunit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/unit/quantity-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/unit/quantity-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/unit/unit-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/unit/unit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.3.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.3.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.4.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.4.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.5.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.5.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/version_map-1.6.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/version_map-1.6.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/celestial_frame-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/celestial_frame-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/celestial_frame-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/celestial_frame-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/composite_frame-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/composite_frame-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/frame-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/frame-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/frame-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/frame-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/icrs_coord-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/icrs_coord-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/spectral_frame-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/spectral_frame-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/spectral_frame-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/spectral_frame-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/step-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.0.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.1.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.2.0.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/asdf/wcs/wcs-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf-standard/schemas/stsci.edu/yaml-schema/draft-01.yaml` & `asdf-2.9.2/asdf-standard/schemas/stsci.edu/yaml-schema/draft-01.yaml`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/asdf.egg-info/PKG-INFO` & `asdf-2.9.2/asdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asdf
-Version: 2.9.1
+Version: 2.9.2
 Summary: Python implementation of the ASDF Standard
 Home-page: http://github.com/asdf-format/asdf
 Author: The ASDF Developers
 Author-email: help@stsci.edu
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/asdf-format/asdf/issues
 Project-URL: Documentation, https://asdf.readthedocs.io/en/stable
```

### Comparing `asdf-2.9.1/asdf.egg-info/SOURCES.txt` & `asdf-2.9.2/asdf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/changelog.yml
 .github/workflows/ci.yml
 .github/workflows/downstream.yml
+.github/workflows/publish-to-pypi.yml
 .github/workflows/s390x.yml
 asdf/__init__.py
 asdf/_convenience.py
 asdf/_display.py
 asdf/_helpers.py
 asdf/asdf.py
 asdf/asdftypes.py
```

### Comparing `asdf-2.9.1/compatibility_tests/README.md` & `asdf-2.9.2/compatibility_tests/README.md`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/compatibility_tests/common.py` & `asdf-2.9.2/compatibility_tests/common.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/compatibility_tests/generate_file.py` & `asdf-2.9.2/compatibility_tests/generate_file.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/compatibility_tests/test_file_compatibility.py` & `asdf-2.9.2/compatibility_tests/test_file_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import urllib.request
-from distutils.version import StrictVersion
+from packaging.version import Version
 from itertools import groupby
 from pathlib import Path
 import subprocess
 from contextlib import contextmanager
 import os
 
 import pytest
@@ -12,26 +12,26 @@
 import virtualenv
 
 import asdf
 
 from common import generate_file, assert_file_correct
 
 
-# Strange version present on pypi that doesn't parse as a StrictVersion
+# Strange version present on pypi that doesn't parse as a Version
 BAD_VERSIONS = {"0"}
 
 # Minimum library version to read files produced by the current
 # version of the code.  We're not maintaining < 2.7.x and bugs in older
 # versions prevent valid files from being read.
-MIN_VERSION_NEW_FILES = StrictVersion("2.7.0")
+MIN_VERSION_NEW_FILES = Version("2.7.0")
 
 # Minimum library version to produce files read by the current
 # version of the code.  Earlier versions aren't able to generate
 # files for all the ASDF Standard versions that they claim to support.
-MIN_VERSION_OLD_FILES = StrictVersion("2.3.0")
+MIN_VERSION_OLD_FILES = Version("2.3.0")
 
 GENERATE_SCRIPT_PATH = Path(__file__).parent/"generate_file.py"
 ASSERT_SCRIPT_PATH = Path(__file__).parent/"assert_file_correct.py"
 
 
 @contextmanager
 def internet_temporarily_enabled(verbose=False):
@@ -52,25 +52,25 @@
 def fetch_package_versions(package_name):
     """
     Request a package's available versions from pypi.org metadata.
     """
     content = urllib.request.urlopen("https://pypi.org/pypi/{}/json".format(package_name)).read()
     version_strings = json.loads(content)["releases"].keys()
     return [
-        StrictVersion(v) for v in version_strings
-        if v not in BAD_VERSIONS and (v >= MIN_VERSION_NEW_FILES or v >= MIN_VERSION_OLD_FILES)
+        Version(v) for v in version_strings
+        if v not in BAD_VERSIONS and (Version(v) >= MIN_VERSION_NEW_FILES or Version(v) >= MIN_VERSION_OLD_FILES)
     ]
 
 
 def fetch_latest_patch_versions(package_name):
     """
     Return the latest patch version within each of the package's
     minor versions.
     """
-    key_fn = lambda v: v.version[0:2]
+    key_fn = lambda v: v.release[0:2]
 
     versions = sorted(fetch_package_versions(package_name), key=key_fn)
     return [max(group) for _, group in groupby(versions, key=key_fn)]
 
 
 # Enable internet here, otherwise pytest_remotedata will complain
 # (and @pytest.mark.remote_data doesn't work on non-test methods).
@@ -106,15 +106,15 @@
 
 def get_installed_version(env_path):
     """
     Get the version of the asdf library installed in the specified
     virtual environment.
     """
     script = r"""import asdf; print(asdf.__version__)"""
-    return StrictVersion(env_check_output(env_path, "python3", "-c", script))
+    return Version(env_check_output(env_path, "python3", "-c", script))
 
 
 @pytest.fixture(scope="module", params=PATCH_VERSIONS)
 def asdf_version(request):
     """
     The (old) version of the asdf library under test.
     """
```

### Comparing `asdf-2.9.1/docker/s390x/Dockerfile` & `asdf-2.9.2/docker/s390x/Dockerfile`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/Makefile` & `asdf-2.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/arrays.rst` & `asdf-2.9.2/docs/asdf/arrays.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/asdf_tool.rst` & `asdf-2.9.2/docs/asdf/asdf_tool.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/changes.rst` & `asdf-2.9.2/docs/asdf/changes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 .. currentmodule:: asdf
 
 *******
 Changes
 *******
 
+What's new in asdf 2.9.2?
+=========================
+
+The ASDF Standard is at v1.6.0.
+
+Changes include:
+
+- Fix deprecation warnings stemming from the release of pytest 7.0.0.
+
+- Fix bug in pytest plugin when schemas are not in a directory named "schemas".
+
 What's new in asdf 2.9.1?
 =========================
 
 The ASDF Standard is at v1.6.0.
 
 Changes include:
```

### Comparing `asdf-2.9.1/docs/asdf/config.rst` & `asdf-2.9.2/docs/asdf/config.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/developer_overview.rst` & `asdf-2.9.2/docs/asdf/developer_overview.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/developer_versioning.rst` & `asdf-2.9.2/docs/asdf/developer_versioning.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/extending/compressors.rst` & `asdf-2.9.2/docs/asdf/extending/compressors.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/extending/converters.rst` & `asdf-2.9.2/docs/asdf/extending/converters.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/extending/extensions.rst` & `asdf-2.9.2/docs/asdf/extending/extensions.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/extending/legacy.rst` & `asdf-2.9.2/docs/asdf/extending/legacy.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/extending/manifests.rst` & `asdf-2.9.2/docs/asdf/extending/manifests.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/extending/resources.rst` & `asdf-2.9.2/docs/asdf/extending/resources.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/extending/schemas.rst` & `asdf-2.9.2/docs/asdf/extending/schemas.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/extending/uris.rst` & `asdf-2.9.2/docs/asdf/extending/uris.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/extending/use_cases.rst` & `asdf-2.9.2/docs/asdf/extending/use_cases.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/features.rst` & `asdf-2.9.2/docs/asdf/features.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/install.rst` & `asdf-2.9.2/docs/asdf/install.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/overview.rst` & `asdf-2.9.2/docs/asdf/overview.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/asdf/using_extensions.rst` & `asdf-2.9.2/docs/asdf/using_extensions.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/conf.py` & `asdf-2.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/index.rst` & `asdf-2.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/make.bat` & `asdf-2.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/docs/sphinxext/example.py` & `asdf-2.9.2/docs/sphinxext/example.py`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/pytest_asdf/plugin.py` & `asdf-2.9.2/pytest_asdf/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import io
 import os
-from importlib.util import find_spec
-from pkg_resources import parse_version
 import pathlib
+import warnings
 
 import yaml
 import pytest
 
 import numpy as np
 
 # Avoid all imports of asdf at this level in order to avoid circular imports
@@ -54,18 +53,28 @@
         help='Enable ASDF schema tests')
 
 
 class AsdfSchemaFile(pytest.File):
     @classmethod
     def from_parent(cls, parent, *, fspath, skip_examples=False, validate_default=True,
         ignore_unrecognized_tag=False, ignore_version_mismatch=False, skip_tests=[], xfail_tests=[], **kwargs):
+
+        # Fix for depreciation of fspath in pytest 7+
+        from asdf.util import minversion
+        if minversion("pytest", "7.0.0"):
+            path = pathlib.Path(fspath)
+            kwargs["path"] = path
+        else:
+            path = fspath
+            kwargs["fspath"] = path
+
         if hasattr(super(), "from_parent"):
-            result = super().from_parent(parent, fspath=fspath, **kwargs)
+            result = super().from_parent(parent, **kwargs)
         else:
-            result = AsdfSchemaFile(fspath, parent, **kwargs)
+            result = AsdfSchemaFile(path, parent)
 
         result.skip_examples = skip_examples
         result.validate_default = validate_default
         result.ignore_unrecognized_tag = ignore_unrecognized_tag
         result.ignore_version_mismatch = ignore_version_mismatch
         result.skip_tests = skip_tests
         result.xfail_tests = xfail_tests
@@ -136,49 +145,14 @@
             resolve_references=True)
         schema.check_schema(schema_tree, validate_default=self.validate_default)
 
     def reportinfo(self):
         return self.fspath, 0, ""
 
 
-ASTROPY_4_0_TAGS = {
-    'tag:stsci.edu:asdf/transform/rotate_sequence_3d',
-    'tag:stsci.edu:asdf/transform/ortho_polynomial',
-    'tag:stsci.edu:asdf/transform/fix_inputs',
-    'tag:stsci.edu:asdf/transform/math_functions',
-    'tag:stsci.edu:asdf/time/time',
-}
-
-
-def should_skip(name, version):
-    if name == 'tag:stsci.edu:asdf/transform/multiplyscale':
-        return not is_min_astropy_version('3.1.dev0')
-    elif name in ASTROPY_4_0_TAGS:
-        return not is_min_astropy_version('4.0')
-
-    return False
-
-
-def is_min_astropy_version(min_version):
-    astropy = find_spec('astropy')
-    if astropy is None:
-        return False
-
-    import astropy
-    return parse_version(astropy.version.version) >= parse_version(min_version)
-
-
-def parse_schema_filename(filename):
-    from asdf import versioning
-    components = filename[filename.find('schemas') + 1:].split(os.path.sep)
-    tag = 'tag:{}:{}'.format(components[1], '/'.join(components[2:]))
-    name, version = versioning.split_tag_version(tag.replace('.yaml', ''))
-    return name, version
-
-
 class AsdfSchemaExampleItem(pytest.Item):
     @classmethod
     def from_parent(cls, parent, schema_path, example, example_index,
         ignore_unrecognized_tag=False, ignore_version_mismatch=False, **kwargs):
         if hasattr(super(), "from_parent"):
             result = super().from_parent(parent, **kwargs)
         else:
@@ -187,37 +161,21 @@
 
         result.filename = str(schema_path)
         result.example = example
         result.ignore_unrecognized_tag = ignore_unrecognized_tag
         result.ignore_version_mismatch = ignore_version_mismatch
         return result
 
-    def _find_standard_version(self, name, version):
-        from asdf import versioning
-        for sv in reversed(versioning.supported_versions):
-            map_version = versioning.get_version_map(sv)['tags'].get(name)
-            if map_version is not None and version == map_version:
-                return sv
-
-        return versioning.default_version
-
     def runtest(self):
         from asdf import AsdfFile, block, util
         from asdf.tests import helpers
 
-        name, version = parse_schema_filename(self.filename)
-        if should_skip(name, version):
-            return
-
-        standard_version = self._find_standard_version(name, version)
-
         # Make sure that the examples in the schema files (and thus the
         # ASDF standard document) are valid.
-        buff = helpers.yaml_to_asdf(
-            'example: ' + self.example.strip(), standard_version=standard_version)
+        buff = helpers.yaml_to_asdf('example: ' + self.example.strip())
 
         ff = AsdfFile(
             uri=util.filepath_to_url(os.path.abspath(self.filename)),
             ignore_unrecognized_tag=self.ignore_unrecognized_tag,
             ignore_version_mismatch=self.ignore_version_mismatch,
         )
 
@@ -234,18 +192,19 @@
         for i in range(3):
             b = block.Block(np.zeros((1024*1024*8), dtype=np.uint8))
             b._used = True
             ff.blocks.add(b)
         b._array_storage = "streamed"
 
         try:
-            with pytest.warns(None) as w:
-                ff._open_impl(ff, buff, mode='rw')
             # Do not tolerate any warnings that occur during schema validation
-            assert len(w) == 0, helpers.display_warnings(w)
+            with warnings.catch_warnings():
+                warnings.simplefilter("error")
+
+                ff._open_impl(ff, buff, mode='rw')
         except Exception:
             print("From file:", self.filename)
             raise
 
         # Just test we can write it out.  A roundtrip test
         # wouldn't always yield the correct result, so those have
         # to be covered by "real" unit tests.
```

### Comparing `asdf-2.9.1/setup.cfg` & `asdf-2.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `asdf-2.9.1/setup.py` & `asdf-2.9.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,21 +16,25 @@
 
 package_dir = {
     'asdf.schemas': 'asdf-standard/schemas',
     'asdf.reference_files': 'asdf-standard/reference_files',
     'asdf.resources': 'asdf-standard/resources',
 }
 
+def package_yaml_files(directory):
+    paths = sorted(Path(directory).rglob("*.yaml"))
+    return [str(p.relative_to(directory)) for p in paths]
+
 package_data = {
     'asdf.commands.tests.data': ['*'],
     'asdf.tags.core.tests.data': ['*'],
     'asdf.tests.data': ['*'],
     'asdf.reference_files': ['*', '**/*'],
-    'asdf.schemas':  ['*.yaml', '**/*.yaml', '**/**/*.yaml', '**/**/**/*.yaml'],
-    'asdf.resources': ['*.yaml', '**/*.yaml', '**/**/*.yaml', '**/**/**/*.yaml'],
+    'asdf.schemas':  package_yaml_files("asdf-standard/schemas"),
+    'asdf.resources': package_yaml_files("asdf-standard/resources"),
 }
 
 setup(
     use_scm_version={"write_to": os.path.join("asdf", "version.py"), "write_to_template": 'version = "{version}"\n'},
     packages=packages,
     package_dir=package_dir,
     package_data=package_data,
```

### Comparing `asdf-2.9.1/tox.ini` & `asdf-2.9.2/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 [testenv]
 deps=
     pytest-sugar
     astropydev: git+https://github.com/astropy/astropy
     gwcsdev: git+https://github.com/spacetelescope/gwcs
     numpydev: git+https://github.com/numpy/numpy
+    asdfastropydev: git+https://github.com/astropy/asdf-astropy
+    asdftransformschemasdev: git+https://github.com/asdf-format/asdf-transform-schemas
+    asdfwcsschemasdev: git+https://github.com/asdf-format/asdf-wcs-schemas
+    asdfcoordinatesschemasdev: git+https://github.com/asdf-format/asdf-coordinates-schemas
     # Newer versions of gwcs require astropy 4.x, which
     # isn't compatible with the older versions of numpy
     # that we test with.
     legacy: gwcs==0.9.1
     legacy: semantic_version==2.8
     legacy: pyyaml==3.13
     legacy: jsonschema==3.0.2
```

