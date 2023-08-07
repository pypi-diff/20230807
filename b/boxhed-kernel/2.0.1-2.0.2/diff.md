# Comparing `tmp/boxhed_kernel-2.0.1.tar.gz` & `tmp/boxhed_kernel-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxhed_kernel-2.0.1.tar", last modified: Fri Jun  9 18:13:13 2023, max compression
+gzip compressed data, was "boxhed_kernel-2.0.2.tar", last modified: Thu Jul 20 02:42:02 2023, max compression
```

## Comparing `boxhed_kernel-2.0.1.tar` & `boxhed_kernel-2.0.2.tar`

### file list

```diff
@@ -1,491 +1,490 @@
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.689172 boxhed_kernel-2.0.1/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      292 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/MANIFEST.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1199 2023-06-09 18:13:13.689172 boxhed_kernel-2.0.1/PKG-INFO
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      492 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/README.rst
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.641173 boxhed_kernel-2.0.1/boxhed_kernel/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12798 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/CMakeLists.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11349 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/LICENSE
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.641173 boxhed_kernel-2.0.1/boxhed_kernel/cmake/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      548 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/Doc.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      683 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/FindPrefetchIntrinsics.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       80 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/Python_version.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1188 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/RPackageInstall.cmake.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      686 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/RPackageInstallTargetSetup.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2194 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/Sanitizer.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6994 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/Utils.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      377 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/Version.cmake
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.645173 boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      410 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindASan.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      362 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindLSan.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6305 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindLibR.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      516 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindNVML.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      581 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindNVTX.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2293 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindNccl.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      362 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindTSan.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      424 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindUBSan.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      304 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/version_config.h.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      466 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/xgboost-config.cmake.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      284 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/cmake/xgboost.pc.in
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.645173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       95 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/.editorconfig
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9094 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/CMakeLists.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11357 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/LICENSE
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2243 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/Makefile
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1940 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/README.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4896 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/appveyor.yml
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.645173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.645173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Modules/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      401 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Modules/FindASan.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2075 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Modules/FindHDFS.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      366 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Modules/FindLSan.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      366 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Modules/FindTSan.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      424 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Modules/FindUBSan.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2048 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Sanitizer.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    13405 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Utils.cmake
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      682 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/build_config.h.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      105 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/dmlc-config.cmake.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      414 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/gtest_cmake.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      821 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/lint.cmake
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.645173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       16 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/.gitignore
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)   105082 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/Doxyfile
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7405 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/Makefile
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      166 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/README
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      477 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/build.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5609 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/conf.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      444 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/index.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8436 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/parameter.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      496 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/sphinx_util.py
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.645173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/example/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      175 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/example/dmlc_example.mk
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1823 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/example/parameter.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.637173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.649173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11286 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/any.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3262 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/array_view.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7447 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/base.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    33014 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/blockingconcurrentqueue.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1241 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/build_config_default.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2240 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/common.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6984 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/concurrency.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)   159320 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/concurrentqueue.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5037 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/config.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12178 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/data.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1984 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/endian.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4883 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/filesystem.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5903 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/input_split_shuffle.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    20386 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/io.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    27908 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/json.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    13523 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/logging.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    21199 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/lua.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6887 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/memory.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2948 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/memory_io.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1146 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/omp.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7209 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/optional.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    38436 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/parameter.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5892 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/recordio.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10305 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/registry.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12463 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/serializer.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    25716 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/strtonum.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    28348 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/thread_group.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2072 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/thread_local.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16578 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/threadediter.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1259 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/timer.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5315 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/type_traits.h
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.649173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/make/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1417 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/make/config.mk
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2050 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/make/dmlc.mk
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.649173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7905 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/lint.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      661 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/packages.mk
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.649173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/s390x/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1099 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/s390x/Dockerfile
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      129 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/s390x/build_via_cmake.sh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2241 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/s390x/ci_build.sh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1466 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/s390x/entrypoint.sh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2188 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/test_script.sh
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.653173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6829 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/config.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.653173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2273 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/basic_row_iter.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4818 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/csv_parser.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4010 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/disk_row_iter.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4373 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/libfm_parser.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5100 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/libsvm_parser.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3880 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/parser.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7323 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/row_block.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4402 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/text_parser.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9468 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.657173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2965 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/azure_filesys.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1272 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/azure_filesys.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6045 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/cached_input_split.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1739 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/filesys.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5512 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/hdfs_filesys.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2636 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/hdfs_filesys.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8333 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/indexed_recordio_split.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2698 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/indexed_recordio_split.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10118 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/input_split_base.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6234 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/input_split_base.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1466 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/line_split.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      996 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/line_split.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6189 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/local_filesys.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2028 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/local_filesys.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3131 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/recordio_split.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1128 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/recordio_split.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    44745 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/s3_filesys.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3183 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/s3_filesys.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4993 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/single_file_split.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2424 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/single_threaded_input_split.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2968 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/threaded_input_split.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2352 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/uri_spec.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4703 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5522 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/recordio.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.661173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       12 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/.gitignore
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      561 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/README.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1722 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/csv_parser_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      784 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/dataiter_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1370 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/dmlc_test.mk
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1717 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/filesys_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      556 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/iostream_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1141 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/libfm_parser_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1098 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/libsvm_parser_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      266 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/logging_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2625 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/parameter_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3674 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/recordio_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1355 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/registry_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1082 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/split_read_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1548 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/split_repeat_read_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      646 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/split_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1234 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/stream_read_test.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1076 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/strtonum_test.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.661173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       29 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/.gitignore
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2911 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/CMakeLists.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       68 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/build_config.h.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      416 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/dmlc_unittest.mk
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      532 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/sample.rec
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1884 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_any.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      455 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_array_view.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2620 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_config.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1262 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_env.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6009 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_inputsplit.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3007 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_json.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4454 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_lockfree.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      334 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_logging.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      214 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_main.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4148 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_optional.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7071 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_param.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    22755 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_parser.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3487 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_serializer.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2493 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_tempdir.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8939 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_thread_group.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1689 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_threaditer.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4383 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_threaditer_exc_handling.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.661173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1508 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/README.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      197 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc-submit
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.665172 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      107 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/__init__.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5875 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/kubernetes.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2802 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/launcher.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2566 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/local.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3112 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/mesos.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2647 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/mpi.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9424 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/opts.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1822 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/sge.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1944 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/slurm.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3271 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/ssh.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1579 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/submit.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16189 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/tracker.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      296 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/util.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5143 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/yarn.py
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.665172 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       30 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/.gitignore
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      216 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/README.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      217 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/build.bat
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      233 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/build.sh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5621 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/pom.xml
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.637173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.637173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.637173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.637173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.637173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.637173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.637173 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.665172 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    27065 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/ApplicationMaster.java
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    14107 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/Client.java
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      888 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/TaskRecord.java
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.665172 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/windows/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       69 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/windows/.gitignore
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      168 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/windows/README.md
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.665172 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/windows/dmlc/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8538 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/windows/dmlc/dmlc.vcxproj
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3073 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/windows/dmlc.sln
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.641173 boxhed_kernel-2.0.1/boxhed_kernel/include/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.665172 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9010 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/base.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    35634 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/c_api.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18768 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/data.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2584 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/feature_map.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8779 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/gbm.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3058 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/generic_parameters.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5396 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/host_device_vector.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5977 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/intrusive_ptr.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16944 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/json.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3039 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/json_io.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9755 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/learner.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2210 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/linear_updater.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5150 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/logging.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3441 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/metric.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1087 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/model.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3711 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/objective.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3034 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/parameter.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9530 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/predictor.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    22993 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/span.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    26186 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/tree_model.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3918 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/tree_updater.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      238 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/version_config.h
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/plugin/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2139 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/CMakeLists.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1620 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/README.md
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/plugin/dense_parser/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2733 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/dense_parser/dense_libsvm.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/plugin/example/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      686 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/example/README.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3235 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/example/custom_obj.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/plugin/lz4/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11615 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/lz4/sparse_page_lz4_format.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_gpu/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      188 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_gpu/README.md
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_oneapi/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1576 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_oneapi/README.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16128 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_oneapi/predictor_oneapi.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5349 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_oneapi/regression_loss_oneapi.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6999 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_oneapi/regression_obj_oneapi.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/rabit/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      429 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/.gitignore
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      504 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/CMakeLists.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1478 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/LICENSE
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      129 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/README.md
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       27 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/.gitignore
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9909 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/Doxyfile
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7405 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/Makefile
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6362 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/conf.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      162 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/cpp_api.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    20561 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/guide.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      652 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/index.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1048 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/parameters.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       25 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/python-requirements.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      182 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/python_api.md
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      496 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/sphinx_util.py
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      774 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/Makefile
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       31 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/README
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1015 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/basic.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      729 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/basic.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      481 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/broadcast.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      538 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/broadcast.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1007 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/lazy_allreduce.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      910 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/lazy_allreduce.py
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.641173 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.669172 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      399 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/base.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7208 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/c_api.h
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.673172 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12725 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/engine.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3307 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/io.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11818 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/rabit-inl.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    17594 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/socket.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3718 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/utils.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    15597 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/rabit.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      616 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/serializable.h
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.673172 boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    35310 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/allreduce_base.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    22866 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/allreduce_base.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6583 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/allreduce_mock.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10544 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/c_api.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3725 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/engine.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      427 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/engine_mock.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7898 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/engine_mpi.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.673172 boxhed_kernel-2.0.1/boxhed_kernel/src/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3130 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/CMakeLists.txt
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.673172 boxhed_kernel-2.0.1/boxhed_kernel/src/c_api/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    31231 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/c_api/c_api.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3753 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/c_api/c_api.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      495 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/c_api/c_api_error.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2047 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/c_api/c_api_error.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16387 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/cli_main.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.677172 boxhed_kernel-2.0.1/boxhed_kernel/src/common/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8031 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/base64.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7644 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/bitfield.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1355 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/categorical.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    35329 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/charconv.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3307 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/charconv.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12717 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/column_matrix.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      743 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/common.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      438 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/common.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4486 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/common.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7103 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/compressed_iterator.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5448 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/config.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3927 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/device_helpers.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    40859 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/device_helpers.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4993 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/group_data.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    30946 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/hist_util.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18923 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/hist_util.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    13033 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/hist_util.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    21336 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/hist_util.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5249 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/host_device_vector.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11740 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/host_device_vector.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4153 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/io.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2543 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/io.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    17993 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/json.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5156 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/math.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4464 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/observer.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3060 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/probability_distribution.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12247 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/quantile.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    29507 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/quantile.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5699 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/quantile.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    25137 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/quantile.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1228 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/random.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6538 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/random.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7787 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/row_set.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      424 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/survival_util.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12125 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/survival_util.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5429 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/threading_utils.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4251 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/timer.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2296 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/timer.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6848 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/transform.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2703 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/version.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      856 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/common/version.h
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.681172 boxhed_kernel-2.0.1/boxhed_kernel/src/data/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    19108 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/adapter.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11991 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/array_interface.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    40106 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/data.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4613 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/data.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7597 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/device_adapter.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      971 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    19044 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7899 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1657 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page_raw_format.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      651 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page_source.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3213 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page_source.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1797 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page_source.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6563 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/iterative_device_dmatrix.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2256 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/iterative_device_dmatrix.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      828 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/proxy_dmatrix.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2967 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/proxy_dmatrix.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      769 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/simple_batch_iterator.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8216 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/simple_dmatrix.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4084 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/simple_dmatrix.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1727 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/simple_dmatrix.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1544 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_dmatrix.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2247 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_dmatrix.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3718 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_raw_format.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2318 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_source.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18953 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_source.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6815 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_writer.h
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.681172 boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10917 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gblinear.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1091 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gblinear_model.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4189 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gblinear_model.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1051 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbm.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    31299 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbtree.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12388 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbtree.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3128 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbtree_model.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4640 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbtree_model.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    44558 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/learner.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.681172 boxhed_kernel-2.0.1/boxhed_kernel/src/linear/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    17840 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/linear/coordinate_common.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      966 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/linear/linear_updater.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2093 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/linear/param.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3897 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/linear/updater_coordinate.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9587 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/linear/updater_gpu_coordinate.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3798 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/linear/updater_shotgun.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2853 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/logging.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.681172 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      208 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/elementwise_metric.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12300 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/elementwise_metric.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2609 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/metric.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2887 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/metric_common.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      207 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/multiclass_metric.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8007 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/multiclass_metric.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    23884 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/rank_metric.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    30100 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/rank_metric.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      329 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/survival_metric.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9608 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/metric/survival_metric.cu
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.685172 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      457 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/aft_obj.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5509 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/aft_obj.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      325 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/hinge.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3180 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/hinge.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      339 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/multiclass_obj.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7086 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/multiclass_obj.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1445 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/objective.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      326 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/rank_obj.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    38856 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/rank_obj.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6224 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/regression_loss.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      339 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/regression_obj.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    25977 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/objective/regression_obj.cu
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.685172 boxhed_kernel-2.0.1/boxhed_kernel/src/predictor/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    22672 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/predictor/cpu_predictor.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    38146 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/predictor/gpu_predictor.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1952 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/predictor/predictor.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.685172 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3451 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/constraints.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12137 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/constraints.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3669 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/constraints.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2013 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/constraints.h
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.689172 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3905 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/driver.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    14255 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/evaluate_splits.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1361 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/evaluate_splits.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1980 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/feature_groups.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4438 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/feature_groups.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    15028 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5305 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9173 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/histogram.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1018 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/histogram.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7083 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/row_partitioner.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7390 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/row_partitioner.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2404 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/param.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    19480 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/param.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6210 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/split_evaluator.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    47842 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/tree_model.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1159 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/tree_updater.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    17542 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_basemaker-inl.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    24673 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_colmaker.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3916 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_gpu_common.cuh
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    36104 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_gpu_hist.cu
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    28961 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_histmaker.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3513 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_prune.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    56259 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_quantile_hist.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    20234 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_quantile_hist.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5665 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_refresh.cc
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1456 2023-06-07 00:34:06.000000 boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_sync.cc
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.641173 boxhed_kernel-2.0.1/boxhed_kernel.egg-info/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1199 2023-06-09 18:13:13.000000 boxhed_kernel-2.0.1/boxhed_kernel.egg-info/PKG-INFO
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18495 2023-06-09 18:13:13.000000 boxhed_kernel-2.0.1/boxhed_kernel.egg-info/SOURCES.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-09 18:13:13.000000 boxhed_kernel-2.0.1/boxhed_kernel.egg-info/dependency_links.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-06-09 18:13:13.000000 boxhed_kernel-2.0.1/boxhed_kernel.egg-info/not-zip-safe
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      145 2023-06-09 18:13:13.000000 boxhed_kernel-2.0.1/boxhed_kernel.egg-info/requires.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       19 2023-06-09 18:13:13.000000 boxhed_kernel-2.0.1/boxhed_kernel.egg-info/top_level.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       80 2023-06-09 18:13:13.689172 boxhed_kernel-2.0.1/setup.cfg
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    13087 2023-06-09 18:13:09.000000 boxhed_kernel-2.0.1/setup.py
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-06-09 18:13:13.689172 boxhed_kernel-2.0.1/xgboost/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       15 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/VERSION
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1022 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/__init__.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    27261 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/callback.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5256 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/compat.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    76766 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/core.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    48273 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/dask.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    28194 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/data.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2607 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/libpath.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8349 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/plotting.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5765 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/rabit.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    54965 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/sklearn.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10949 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/tracker.py
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    21658 2023-06-07 00:34:05.000000 boxhed_kernel-2.0.1/xgboost/training.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.312240 boxhed_kernel-2.0.2/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      304 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/MANIFEST.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      740 2023-07-20 02:42:02.312240 boxhed_kernel-2.0.2/PKG-INFO
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:41:22.000000 boxhed_kernel-2.0.2/README.rst
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.272241 boxhed_kernel-2.0.2/boxhed_kernel/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    13302 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/CMakeLists.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11349 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/LICENSE
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       15 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/VERSION
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1028 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/__init__.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    27267 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/callback.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.276241 boxhed_kernel-2.0.2/boxhed_kernel/cmake/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      554 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/Doc.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      683 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/FindPrefetchIntrinsics.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       98 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/Python_version.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1188 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/RPackageInstall.cmake.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      692 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/RPackageInstallTargetSetup.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2194 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/Sanitizer.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7012 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/Utils.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      425 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/Version.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      484 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/boxhed_kernel-config.cmake.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      302 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/boxhed_kernel.pc.in
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.276241 boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      410 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindASan.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      362 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindLSan.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6305 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindLibR.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      516 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindNVML.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      581 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindNVTX.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2293 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindNccl.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      362 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindTSan.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      424 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindUBSan.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      322 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/cmake/version_config.h.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5256 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/compat.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    76826 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/core.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    48369 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dask.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    28194 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/data.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.276241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       95 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/.editorconfig
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9094 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/CMakeLists.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11357 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/LICENSE
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2243 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/Makefile
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1940 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/README.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4896 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/appveyor.yml
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.276241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.276241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Modules/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      401 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Modules/FindASan.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2075 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Modules/FindHDFS.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      366 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Modules/FindLSan.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      366 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Modules/FindTSan.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      424 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Modules/FindUBSan.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2048 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Sanitizer.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    13405 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Utils.cmake
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      682 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/build_config.h.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      105 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/dmlc-config.cmake.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      414 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/gtest_cmake.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      821 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/lint.cmake
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.276241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       16 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/.gitignore
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)   105082 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/Doxyfile
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7405 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/Makefile
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      166 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/README
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      477 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/build.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5609 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/conf.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      444 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/index.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8436 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/parameter.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      496 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/sphinx_util.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.276241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/example/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      175 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/example/dmlc_example.mk
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1823 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/example/parameter.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.268241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.280241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11286 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/any.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3262 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/array_view.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7447 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/base.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    33014 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/blockingconcurrentqueue.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1241 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/build_config_default.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2240 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/common.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6984 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/concurrency.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)   159320 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/concurrentqueue.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5037 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/config.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12178 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/data.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1984 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/endian.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4883 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/filesystem.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5903 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/input_split_shuffle.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    20386 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/io.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    27908 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/json.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    13523 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/logging.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    21199 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/lua.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6887 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/memory.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2948 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/memory_io.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1146 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/omp.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7209 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/optional.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    38436 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/parameter.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5892 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/recordio.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10305 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/registry.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12463 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/serializer.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    25716 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/strtonum.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    28348 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/thread_group.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2072 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/thread_local.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16578 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/threadediter.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1259 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/timer.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5315 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/type_traits.h
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.280241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/make/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1417 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/make/config.mk
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2050 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/make/dmlc.mk
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.280241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7905 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/lint.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      661 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/packages.mk
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.280241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/s390x/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1099 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/s390x/Dockerfile
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      129 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/s390x/build_via_cmake.sh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2241 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/s390x/ci_build.sh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1466 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/s390x/entrypoint.sh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2188 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/test_script.sh
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.284241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6829 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/config.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.284241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2273 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/basic_row_iter.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4818 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/csv_parser.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4010 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/disk_row_iter.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4373 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/libfm_parser.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5100 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/libsvm_parser.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3880 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/parser.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7323 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/row_block.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4402 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/text_parser.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9468 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.284241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2965 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/azure_filesys.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1272 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/azure_filesys.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6045 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/cached_input_split.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1739 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/filesys.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5512 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/hdfs_filesys.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2636 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/hdfs_filesys.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8333 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/indexed_recordio_split.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2698 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/indexed_recordio_split.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10118 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/input_split_base.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6234 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/input_split_base.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1466 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/line_split.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      996 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/line_split.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6189 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/local_filesys.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2028 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/local_filesys.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3131 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/recordio_split.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1128 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/recordio_split.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    44745 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/s3_filesys.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3183 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/s3_filesys.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4993 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/single_file_split.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2424 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/single_threaded_input_split.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2968 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/threaded_input_split.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2352 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/uri_spec.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4703 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5522 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/recordio.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.288241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       12 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/.gitignore
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      561 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/README.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1722 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/csv_parser_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      784 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/dataiter_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1370 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/dmlc_test.mk
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1717 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/filesys_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      556 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/iostream_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1141 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/libfm_parser_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1098 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/libsvm_parser_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      266 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/logging_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2625 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/parameter_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3674 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/recordio_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1355 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/registry_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1082 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/split_read_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1548 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/split_repeat_read_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      646 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/split_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1234 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/stream_read_test.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1076 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/strtonum_test.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.288241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       29 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/.gitignore
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2911 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/CMakeLists.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       68 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/build_config.h.in
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      416 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/dmlc_unittest.mk
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      532 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/sample.rec
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1884 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_any.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      455 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_array_view.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2620 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_config.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1262 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_env.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6009 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_inputsplit.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3007 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_json.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4454 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_lockfree.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      334 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_logging.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      214 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_main.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4148 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_optional.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7071 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_param.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    22755 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_parser.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3487 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_serializer.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2493 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_tempdir.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8939 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_thread_group.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1689 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_threaditer.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4383 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_threaditer_exc_handling.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.288241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1508 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/README.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      197 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc-submit
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.292241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      107 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/__init__.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5875 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/kubernetes.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2802 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/launcher.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2566 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/local.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3112 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/mesos.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2647 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/mpi.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9424 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/opts.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1822 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/sge.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1944 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/slurm.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3271 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/ssh.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1579 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/submit.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16189 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/tracker.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      296 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/util.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5143 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/yarn.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.292241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       30 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/.gitignore
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      216 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/README.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      217 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/build.bat
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      233 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/build.sh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5621 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/pom.xml
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.268241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.268241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.268241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.268241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.268241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.268241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.268241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.292241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    27065 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/ApplicationMaster.java
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    14107 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/Client.java
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      888 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/TaskRecord.java
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.292241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/windows/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       69 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/windows/.gitignore
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      168 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/windows/README.md
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.292241 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/windows/dmlc/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8538 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/windows/dmlc/dmlc.vcxproj
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3073 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/windows/dmlc.sln
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.268241 boxhed_kernel-2.0.2/boxhed_kernel/include/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.292241 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9034 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/base.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    35658 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/c_api.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18840 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/data.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2602 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/feature_map.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8827 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/gbm.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3082 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/generic_parameters.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5414 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/host_device_vector.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6013 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/intrusive_ptr.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16980 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/json.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3063 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/json_io.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9809 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/learner.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2264 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/linear_updater.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5270 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/logging.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3501 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/metric.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1099 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/model.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3771 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/objective.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3052 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/parameter.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9584 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/predictor.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    23029 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/span.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    26234 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/tree_model.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3978 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/tree_updater.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      238 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/version_config.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2667 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/libpath.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8349 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plotting.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.292241 boxhed_kernel-2.0.2/boxhed_kernel/plugin/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2241 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/CMakeLists.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1662 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/README.md
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.292241 boxhed_kernel-2.0.2/boxhed_kernel/plugin/dense_parser/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2745 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/dense_parser/dense_libsvm.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.296241 boxhed_kernel-2.0.2/boxhed_kernel/plugin/example/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      722 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/example/README.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3283 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/example/custom_obj.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.296241 boxhed_kernel-2.0.2/boxhed_kernel/plugin/lz4/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11645 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/lz4/sparse_page_lz4_format.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.296241 boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_gpu/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      194 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_gpu/README.md
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.296241 boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_oneapi/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1582 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_oneapi/README.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16182 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_oneapi/predictor_oneapi.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5367 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_oneapi/regression_loss_oneapi.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7047 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_oneapi/regression_obj_oneapi.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.296241 boxhed_kernel-2.0.2/boxhed_kernel/rabit/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      429 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/.gitignore
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      504 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/CMakeLists.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1478 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/LICENSE
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      129 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/README.md
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.296241 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       27 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/.gitignore
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9909 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/Doxyfile
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7405 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/Makefile
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6362 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/conf.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      162 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/cpp_api.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    20561 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/guide.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      652 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/index.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1048 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/parameters.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       25 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/python-requirements.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      182 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/python_api.md
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      496 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/sphinx_util.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.296241 boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      774 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/Makefile
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       31 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/README
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1015 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/basic.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      729 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/basic.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      481 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/broadcast.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      538 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/broadcast.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1007 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/lazy_allreduce.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      910 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/lazy_allreduce.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.272241 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.296241 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      399 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/base.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7208 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/c_api.h
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.296241 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12725 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/engine.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3307 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/io.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11818 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/rabit-inl.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    17594 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/socket.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3730 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/utils.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    15597 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/rabit.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      616 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/serializable.h
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.300241 boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    35310 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/allreduce_base.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    22866 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/allreduce_base.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6583 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/allreduce_mock.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10544 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/c_api.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3725 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/engine.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      427 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/engine_mock.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7898 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/engine_mpi.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5765 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/rabit.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    55067 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/sklearn.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.300241 boxhed_kernel-2.0.2/boxhed_kernel/src/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3280 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/CMakeLists.txt
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.300241 boxhed_kernel-2.0.2/boxhed_kernel/src/c_api/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    31753 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/c_api/c_api.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3813 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/c_api/c_api.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      501 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/c_api/c_api_error.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2047 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/c_api/c_api_error.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16477 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/cli_main.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.304241 boxhed_kernel-2.0.2/boxhed_kernel/src/common/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8049 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/base64.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7662 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/bitfield.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1391 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/categorical.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    35347 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/charconv.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3325 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/charconv.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12741 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/column_matrix.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      761 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/common.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      450 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/common.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4510 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/common.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7121 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/compressed_iterator.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5466 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/config.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3969 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/device_helpers.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    41093 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/device_helpers.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5011 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/group_data.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    30994 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/hist_util.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18947 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/hist_util.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    13045 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/hist_util.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    21378 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/hist_util.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5285 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/host_device_vector.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    11770 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/host_device_vector.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4171 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/io.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2555 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/io.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18029 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/json.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5174 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/math.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4506 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/observer.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3072 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/probability_distribution.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12259 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/quantile.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    29525 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/quantile.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5723 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/quantile.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    25161 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/quantile.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1240 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/random.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6574 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/random.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7805 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/row_set.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      436 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/survival_util.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12149 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/survival_util.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5447 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/threading_utils.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4269 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/timer.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2314 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/timer.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6878 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/transform.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2733 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/version.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      874 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/common/version.h
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.308241 boxhed_kernel-2.0.2/boxhed_kernel/src/data/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    19150 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/adapter.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12033 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/array_interface.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    40322 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/data.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4643 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/data.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7609 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/device_adapter.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      989 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    19062 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7917 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1675 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page_raw_format.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      669 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page_source.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3225 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page_source.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1815 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page_source.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6575 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/iterative_device_dmatrix.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2286 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/iterative_device_dmatrix.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      840 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/proxy_dmatrix.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3003 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/proxy_dmatrix.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      787 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/simple_batch_iterator.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8240 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/simple_dmatrix.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4102 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/simple_dmatrix.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1751 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/simple_dmatrix.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1556 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_dmatrix.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2265 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_dmatrix.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3736 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_raw_format.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2330 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_source.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18995 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_source.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6833 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_writer.h
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.308241 boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10965 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gblinear.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1109 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gblinear_model.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4237 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gblinear_model.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1105 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbm.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    31359 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbtree.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12484 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbtree.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3152 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbtree_model.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4676 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbtree_model.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    44678 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/learner.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.308241 boxhed_kernel-2.0.2/boxhed_kernel/src/linear/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    17864 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/linear/coordinate_common.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1008 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/linear/linear_updater.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2111 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/linear/param.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3921 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/linear/updater_coordinate.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9641 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/linear/updater_gpu_coordinate.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3816 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/linear/updater_shotgun.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2901 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/logging.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.308241 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      208 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/elementwise_metric.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12318 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/elementwise_metric.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2657 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/metric.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2917 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/metric_common.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      207 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/multiclass_metric.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     8025 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/multiclass_metric.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    23986 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/rank_metric.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    30142 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/rank_metric.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      329 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/survival_metric.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9656 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/metric/survival_metric.cu
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.308241 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      469 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/aft_obj.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5575 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/aft_obj.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      337 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/hinge.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3216 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/hinge.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      351 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/multiclass_obj.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7128 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/multiclass_obj.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1499 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/objective.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      338 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/rank_obj.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    38892 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/rank_obj.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6242 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/regression_loss.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      351 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/regression_obj.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    26025 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/objective/regression_obj.cu
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.308241 boxhed_kernel-2.0.2/boxhed_kernel/src/predictor/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    22726 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/predictor/cpu_predictor.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    38194 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/predictor/gpu_predictor.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2000 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/predictor/predictor.cc
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.312240 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3475 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/constraints.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12161 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/constraints.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3687 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/constraints.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2037 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/constraints.h
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.312240 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3923 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/driver.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    14267 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/evaluate_splits.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1379 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/evaluate_splits.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1998 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/feature_groups.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     4462 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/feature_groups.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    15052 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5335 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     9191 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/histogram.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1030 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/histogram.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7095 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/row_partitioner.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     7408 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/row_partitioner.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2422 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/param.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    19510 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/param.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     6983 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/split_evaluator.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    47908 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/tree_model.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1207 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/tree_updater.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    17572 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_basemaker-inl.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    24709 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_colmaker.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3928 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_gpu_common.cuh
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    38812 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_gpu_hist.cu
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    28991 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_histmaker.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     3543 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_prune.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    56295 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_quantile_hist.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    20330 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_quantile_hist.h
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     5707 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_refresh.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     1480 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_sync.cc
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    10955 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/tracker.py
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    21664 2023-07-20 02:26:31.000000 boxhed_kernel-2.0.2/boxhed_kernel/training.py
+drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-07-20 02:42:02.272241 boxhed_kernel-2.0.2/boxhed_kernel.egg-info/
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      740 2023-07-20 02:42:02.000000 boxhed_kernel-2.0.2/boxhed_kernel.egg-info/PKG-INFO
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    18717 2023-07-20 02:42:02.000000 boxhed_kernel-2.0.2/boxhed_kernel.egg-info/SOURCES.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-07-20 02:42:02.000000 boxhed_kernel-2.0.2/boxhed_kernel.egg-info/dependency_links.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-07-20 02:42:02.000000 boxhed_kernel-2.0.2/boxhed_kernel.egg-info/not-zip-safe
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      145 2023-07-20 02:42:02.000000 boxhed_kernel-2.0.2/boxhed_kernel.egg-info/requires.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       31 2023-07-20 02:42:02.000000 boxhed_kernel-2.0.2/boxhed_kernel.egg-info/top_level.txt
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       80 2023-07-20 02:42:02.312240 boxhed_kernel-2.0.2/setup.cfg
+-rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    12610 2023-07-20 02:33:06.000000 boxhed_kernel-2.0.2/setup.py
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/CMakeLists.txt` & `boxhed_kernel-2.0.2/boxhed_kernel/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cmake_minimum_required(VERSION 3.13)
-project(xgboost LANGUAGES CXX C VERSION 1.3.0)
+project(boxhed_kernel LANGUAGES CXX C VERSION 1.3.0)
 include(cmake/Utils.cmake)
-list(APPEND CMAKE_MODULE_PATH "${xgboost_SOURCE_DIR}/cmake/modules")
+list(APPEND CMAKE_MODULE_PATH "${boxhed_kernel_SOURCE_DIR}/cmake/modules")
 cmake_policy(SET CMP0022 NEW)
 cmake_policy(SET CMP0079 NEW)
 set(CMAKE_POLICY_DEFAULT_CMP0063 NEW)
 cmake_policy(SET CMP0063 NEW)
 
 if ((${CMAKE_VERSION} VERSION_GREATER 3.13) OR (${CMAKE_VERSION} VERSION_EQUAL 3.13))
   cmake_policy(SET CMP0077 NEW)
@@ -13,17 +13,17 @@
 
 message(STATUS "CMake version ${CMAKE_VERSION}")
 
 if (CMAKE_COMPILER_IS_GNUCC AND CMAKE_CXX_COMPILER_VERSION VERSION_LESS 5.0)
   message(FATAL_ERROR "GCC version must be at least 5.0!")
 endif()
 
-include(${xgboost_SOURCE_DIR}/cmake/FindPrefetchIntrinsics.cmake)
+include(${boxhed_kernel_SOURCE_DIR}/cmake/FindPrefetchIntrinsics.cmake)
 find_prefetch_intrinsics()
-include(${xgboost_SOURCE_DIR}/cmake/Version.cmake)
+include(${boxhed_kernel_SOURCE_DIR}/cmake/Version.cmake)
 write_version()
 set_default_configuration_release()
 
 #-- Options
 ## User options
 option(BUILD_C_DOC "Build documentation for C APIs using Doxygen." OFF)
 option(USE_OPENMP "Build with OpenMP support." ON)
@@ -63,15 +63,15 @@
 address, leak, undefined and thread.")
 ## Plugins
 option(PLUGIN_LZ4 "Build lz4 plugin" OFF)
 option(PLUGIN_DENSE_PARSER "Build dense parser plugin" OFF)
 option(PLUGIN_RMM "Build with RAPIDS Memory Manager (RMM)" OFF)
 ## TODO: 1. Add check if DPC++ compiler is used for building
 option(PLUGIN_UPDATER_ONEAPI "DPC++ updater" OFF)
-option(ADD_PKGCONFIG "Add xgboost.pc into system." ON)
+option(ADD_PKGCONFIG "Add boxhed_kernel.pc into system." ON)
 
 #-- Checks for building XGBoost
 if (USE_DEBUG_OUTPUT AND (NOT (CMAKE_BUILD_TYPE MATCHES Debug)))
   message(SEND_ERROR "Do not enable `USE_DEBUG_OUTPUT' with release build.")
 endif (USE_DEBUG_OUTPUT AND (NOT (CMAKE_BUILD_TYPE MATCHES Debug)))
 if (USE_NCCL AND NOT (USE_CUDA))
   message(SEND_ERROR "`USE_NCCL` must be enabled with `USE_CUDA` flag.")
@@ -103,15 +103,15 @@
 endif (PLUGIN_RMM AND NOT (CMAKE_SYSTEM_NAME STREQUAL "Linux"))
 if (ENABLE_ALL_WARNINGS)
   if ((NOT CMAKE_CXX_COMPILER_ID MATCHES "Clang") AND (NOT CMAKE_CXX_COMPILER_ID STREQUAL "GNU"))
     message(SEND_ERROR "ENABLE_ALL_WARNINGS is only available for Clang and GCC.")
   endif ((NOT CMAKE_CXX_COMPILER_ID MATCHES "Clang") AND (NOT CMAKE_CXX_COMPILER_ID STREQUAL "GNU"))
 endif (ENABLE_ALL_WARNINGS)
 if (BUILD_STATIC_LIB AND (R_LIB OR JVM_BINDINGS))
-  message(SEND_ERROR "Cannot build a static library libxgboost.a when R or JVM packages are enabled.")
+  message(SEND_ERROR "Cannot build a static library libboxhed_kernel.a when R or JVM packages are enabled.")
 endif (BUILD_STATIC_LIB AND (R_LIB OR JVM_BINDINGS))
 
 #-- Sanitizer
 if (USE_SANITIZER)
   include(cmake/Sanitizer.cmake)
   enable_sanitizers("${ENABLED_SANITIZERS}")
 endif (USE_SANITIZER)
@@ -138,23 +138,23 @@
 endif()
 
 find_package(Threads REQUIRED)
 
 if (USE_OPENMP)
   if (APPLE)
     # Require CMake 3.16+ on Mac OSX, as previous versions of CMake had trouble locating
-    # OpenMP on Mac. See https://github.com/dmlc/xgboost/pull/5146#issuecomment-568312706
+    # OpenMP on Mac. See https://github.com/dmlc/boxhed_kernel/pull/5146#issuecomment-568312706
     cmake_minimum_required(VERSION 3.16)
   endif (APPLE)
   find_package(OpenMP REQUIRED)
 endif (USE_OPENMP)
 
 # dmlc-core
 msvc_use_static_runtime()
-add_subdirectory(${xgboost_SOURCE_DIR}/dmlc-core)
+add_subdirectory(${boxhed_kernel_SOURCE_DIR}/dmlc-core)
 set_target_properties(dmlc PROPERTIES
   CXX_STANDARD 14
   CXX_STANDARD_REQUIRED ON
   POSITION_INDEPENDENT_CODE ON)
 if (MSVC)
   target_compile_options(dmlc PRIVATE
                          -D_CRT_SECURE_NO_WARNINGS -D_CRT_SECURE_NO_DEPRECATE)
@@ -166,173 +166,173 @@
 if (ENABLE_ALL_WARNINGS)
   target_compile_options(dmlc PRIVATE -Wall -Wextra)
 endif (ENABLE_ALL_WARNINGS)
 
 # rabit
 add_subdirectory(rabit)
 
-# core xgboost
-add_subdirectory(${xgboost_SOURCE_DIR}/src)
-target_link_libraries(objxgboost PUBLIC dmlc)
+# core boxhed_kernel
+add_subdirectory(${boxhed_kernel_SOURCE_DIR}/src)
+target_link_libraries(objboxhed_kernel PUBLIC dmlc)
 
 # Exports some R specific definitions and objects
 if (R_LIB)
-  add_subdirectory(${xgboost_SOURCE_DIR}/R-package)
+  add_subdirectory(${boxhed_kernel_SOURCE_DIR}/R-package)
 endif (R_LIB)
 
 # Plugin
-add_subdirectory(${xgboost_SOURCE_DIR}/plugin)
+add_subdirectory(${boxhed_kernel_SOURCE_DIR}/plugin)
 
 #-- library
 if (BUILD_STATIC_LIB)
-  add_library(xgboost STATIC)
+  add_library(boxhed_kernel STATIC)
 else (BUILD_STATIC_LIB)
-  add_library(xgboost SHARED)
+  add_library(boxhed_kernel SHARED)
 endif (BUILD_STATIC_LIB)
-target_link_libraries(xgboost PRIVATE objxgboost)
+target_link_libraries(boxhed_kernel PRIVATE objboxhed_kernel)
 
 if (USE_CUDA)
-  xgboost_set_cuda_flags(xgboost)
+  boxhed_kernel_set_cuda_flags(boxhed_kernel)
 endif (USE_CUDA)
 
 #-- Hide all C++ symbols
 if (HIDE_CXX_SYMBOLS)
-  foreach(target objxgboost xgboost dmlc)
+  foreach(target objboxhed_kernel boxhed_kernel dmlc)
     set_target_properties(${target} PROPERTIES CXX_VISIBILITY_PRESET hidden)
   endforeach()
 endif (HIDE_CXX_SYMBOLS)
 
-target_include_directories(xgboost
+target_include_directories(boxhed_kernel
   INTERFACE
   $<INSTALL_INTERFACE:${CMAKE_INSTALL_PREFIX}/include>
   $<BUILD_INTERFACE:${CMAKE_CURRENT_LIST_DIR}/include>)
 
-# This creates its own shared library `xgboost4j'.
+# This creates its own shared library `boxhed_kernel4j'.
 if (JVM_BINDINGS)
-  add_subdirectory(${xgboost_SOURCE_DIR}/jvm-packages)
+  add_subdirectory(${boxhed_kernel_SOURCE_DIR}/jvm-packages)
 endif (JVM_BINDINGS)
 #-- End shared library
 
-#-- CLI for xgboost
-add_executable(runxgboost ${xgboost_SOURCE_DIR}/src/cli_main.cc)
-target_link_libraries(runxgboost PRIVATE objxgboost)
+#-- CLI for boxhed_kernel
+add_executable(runboxhed_kernel ${boxhed_kernel_SOURCE_DIR}/src/cli_main.cc)
+target_link_libraries(runboxhed_kernel PRIVATE objboxhed_kernel)
 if (USE_NVTX)
-  enable_nvtx(runxgboost)
+  enable_nvtx(runboxhed_kernel)
 endif (USE_NVTX)
 
-target_include_directories(runxgboost
+target_include_directories(runboxhed_kernel
   PRIVATE
-  ${xgboost_SOURCE_DIR}/include
-  ${xgboost_SOURCE_DIR}/dmlc-core/include
-  ${xgboost_SOURCE_DIR}/rabit/include)
+  ${boxhed_kernel_SOURCE_DIR}/include
+  ${boxhed_kernel_SOURCE_DIR}/dmlc-core/include
+  ${boxhed_kernel_SOURCE_DIR}/rabit/include)
 set_target_properties(
-  runxgboost PROPERTIES
-  OUTPUT_NAME xgboost
+  runboxhed_kernel PROPERTIES
+  OUTPUT_NAME boxhed_kernel
   CXX_STANDARD 14
   CXX_STANDARD_REQUIRED ON)
-#-- End CLI for xgboost
+#-- End CLI for boxhed_kernel
 
-set_output_directory(runxgboost ${xgboost_SOURCE_DIR})
-set_output_directory(xgboost ${xgboost_SOURCE_DIR}/lib)
+set_output_directory(runboxhed_kernel ${boxhed_kernel_SOURCE_DIR})
+set_output_directory(boxhed_kernel ${boxhed_kernel_SOURCE_DIR}/lib)
 # Ensure these two targets do not build simultaneously, as they produce outputs with conflicting names
-add_dependencies(xgboost runxgboost)
+add_dependencies(boxhed_kernel runboxhed_kernel)
 
 #-- Installing XGBoost
 if (R_LIB)
   include(cmake/RPackageInstallTargetSetup.cmake)
-  set_target_properties(xgboost PROPERTIES PREFIX "")
+  set_target_properties(boxhed_kernel PROPERTIES PREFIX "")
   if (APPLE)
-    set_target_properties(xgboost PROPERTIES SUFFIX ".so")
+    set_target_properties(boxhed_kernel PROPERTIES SUFFIX ".so")
   endif (APPLE)
-  setup_rpackage_install_target(xgboost "${CMAKE_CURRENT_BINARY_DIR}/R-package-install")
+  setup_rpackage_install_target(boxhed_kernel "${CMAKE_CURRENT_BINARY_DIR}/R-package-install")
   set(CMAKE_INSTALL_PREFIX "${CMAKE_CURRENT_BINARY_DIR}/dummy_inst")
 endif (R_LIB)
 if (MINGW)
-  set_target_properties(xgboost PROPERTIES PREFIX "")
+  set_target_properties(boxhed_kernel PROPERTIES PREFIX "")
 endif (MINGW)
 
 if (BUILD_C_DOC)
   include(cmake/Doc.cmake)
   run_doxygen()
 endif (BUILD_C_DOC)
 
 include(GNUInstallDirs)
 # Install all headers.  Please note that currently the C++ headers does not form an "API".
-install(DIRECTORY ${xgboost_SOURCE_DIR}/include/xgboost
+install(DIRECTORY ${boxhed_kernel_SOURCE_DIR}/include/boxhed_kernel
   DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
 
-# Install libraries. If `xgboost` is a static lib, specify `objxgboost` also, to avoid the
+# Install libraries. If `boxhed_kernel` is a static lib, specify `objboxhed_kernel` also, to avoid the
 # following error:
 #
-#  > install(EXPORT ...) includes target "xgboost" which requires target "objxgboost" that is not
+#  > install(EXPORT ...) includes target "boxhed_kernel" which requires target "objboxhed_kernel" that is not
 #  > in any export set.
 #
-# https://github.com/dmlc/xgboost/issues/6085
+# https://github.com/dmlc/boxhed_kernel/issues/6085
 if (BUILD_STATIC_LIB)
-  set(INSTALL_TARGETS xgboost runxgboost objxgboost dmlc)
+  set(INSTALL_TARGETS boxhed_kernel runboxhed_kernel objboxhed_kernel dmlc)
 else (BUILD_STATIC_LIB)
-  set(INSTALL_TARGETS xgboost runxgboost)
+  set(INSTALL_TARGETS boxhed_kernel runboxhed_kernel)
 endif (BUILD_STATIC_LIB)
 
 install(TARGETS ${INSTALL_TARGETS}
   EXPORT XGBoostTargets
   ARCHIVE DESTINATION ${CMAKE_INSTALL_LIBDIR}
   LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
   RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
   INCLUDES DESTINATION ${LIBLEGACY_INCLUDE_DIRS})
 install(EXPORT XGBoostTargets
   FILE XGBoostTargets.cmake
-  NAMESPACE xgboost::
-  DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/xgboost)
+  NAMESPACE boxhed_kernel::
+  DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/boxhed_kernel)
 
 include(CMakePackageConfigHelpers)
 configure_package_config_file(
-  ${CMAKE_CURRENT_LIST_DIR}/cmake/xgboost-config.cmake.in
-  ${CMAKE_CURRENT_BINARY_DIR}/cmake/xgboost-config.cmake
-  INSTALL_DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/xgboost)
+  ${CMAKE_CURRENT_LIST_DIR}/cmake/boxhed_kernel-config.cmake.in
+  ${CMAKE_CURRENT_BINARY_DIR}/cmake/boxhed_kernel-config.cmake
+  INSTALL_DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/boxhed_kernel)
 write_basic_package_version_file(
-  ${CMAKE_BINARY_DIR}/cmake/xgboost-config-version.cmake
+  ${CMAKE_BINARY_DIR}/cmake/boxhed_kernel-config-version.cmake
   VERSION ${XGBOOST_VERSION}
   COMPATIBILITY AnyNewerVersion)
 install(
   FILES
-  ${CMAKE_BINARY_DIR}/cmake/xgboost-config.cmake
-  ${CMAKE_BINARY_DIR}/cmake/xgboost-config-version.cmake
-  DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/xgboost)
+  ${CMAKE_BINARY_DIR}/cmake/boxhed_kernel-config.cmake
+  ${CMAKE_BINARY_DIR}/cmake/boxhed_kernel-config-version.cmake
+  DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/boxhed_kernel)
 
 #-- Test
 if (GOOGLE_TEST)
   enable_testing()
   # Unittests.
-  add_subdirectory(${xgboost_SOURCE_DIR}/tests/cpp)
+  add_subdirectory(${boxhed_kernel_SOURCE_DIR}/tests/cpp)
   add_test(
     NAME TestXGBoostLib
-    COMMAND testxgboost
-    WORKING_DIRECTORY ${xgboost_BINARY_DIR})
+    COMMAND testboxhed_kernel
+    WORKING_DIRECTORY ${boxhed_kernel_BINARY_DIR})
 
   # CLI tests
   configure_file(
-    ${xgboost_SOURCE_DIR}/tests/cli/machine.conf.in
-    ${xgboost_BINARY_DIR}/tests/cli/machine.conf
+    ${boxhed_kernel_SOURCE_DIR}/tests/cli/machine.conf.in
+    ${boxhed_kernel_BINARY_DIR}/tests/cli/machine.conf
     @ONLY)
   add_test(
     NAME TestXGBoostCLI
-    COMMAND runxgboost ${xgboost_BINARY_DIR}/tests/cli/machine.conf
-    WORKING_DIRECTORY ${xgboost_BINARY_DIR})
+    COMMAND runboxhed_kernel ${boxhed_kernel_BINARY_DIR}/tests/cli/machine.conf
+    WORKING_DIRECTORY ${boxhed_kernel_BINARY_DIR})
   set_tests_properties(TestXGBoostCLI
     PROPERTIES
     PASS_REGULAR_EXPRESSION ".*test-rmse:0.087.*")
 endif (GOOGLE_TEST)
 
 # For MSVC: Call msvc_use_static_runtime() once again to completely
-# replace /MD with /MT. See https://github.com/dmlc/xgboost/issues/4462
+# replace /MD with /MT. See https://github.com/dmlc/boxhed_kernel/issues/4462
 # for issues caused by mixing of /MD and /MT flags
 msvc_use_static_runtime()
 
-# Add xgboost.pc
+# Add boxhed_kernel.pc
 if (ADD_PKGCONFIG)
-  configure_file(${xgboost_SOURCE_DIR}/cmake/xgboost.pc.in ${xgboost_BINARY_DIR}/xgboost.pc @ONLY)
+  configure_file(${boxhed_kernel_SOURCE_DIR}/cmake/boxhed_kernel.pc.in ${boxhed_kernel_BINARY_DIR}/boxhed_kernel.pc @ONLY)
 
   install(
-    FILES ${xgboost_BINARY_DIR}/xgboost.pc
+    FILES ${boxhed_kernel_BINARY_DIR}/boxhed_kernel.pc
     DESTINATION ${CMAKE_INSTALL_LIBDIR}/pkgconfig)
 endif (ADD_PKGCONFIG)
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/LICENSE` & `boxhed_kernel-2.0.2/boxhed_kernel/LICENSE`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/Doc.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/Doc.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   find_package(Doxygen REQUIRED)
 
   if (NOT DOXYGEN_DOT_FOUND)
     message(FATAL_ERROR "Command `dot` not found.  Please install graphviz.")
   endif (NOT DOXYGEN_DOT_FOUND)
 
   configure_file(
-    ${xgboost_SOURCE_DIR}/doc/Doxyfile.in
+    ${boxhed_kernel_SOURCE_DIR}/doc/Doxyfile.in
     ${CMAKE_CURRENT_BINARY_DIR}/Doxyfile @ONLY)
   add_custom_target( doc_doxygen ALL
     COMMAND ${DOXYGEN_EXECUTABLE} ${CMAKE_CURRENT_BINARY_DIR}/Doxyfile
     WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}
     COMMENT "Generate C APIs documentation."
     VERBATIM)
 endfunction (run_doxygen)
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/FindPrefetchIntrinsics.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/FindPrefetchIntrinsics.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/RPackageInstall.cmake.in` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/RPackageInstall.cmake.in`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/RPackageInstallTargetSetup.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/RPackageInstallTargetSetup.cmake`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Assembles the R-package files in build_dir;
 # if necessary, installs the main R package dependencies;
 # runs R CMD INSTALL.
 function(setup_rpackage_install_target rlib_target build_dir)
   configure_file(${PROJECT_SOURCE_DIR}/cmake/RPackageInstall.cmake.in ${PROJECT_BINARY_DIR}/RPackageInstall.cmake @ONLY)
   install(
-    DIRECTORY "${xgboost_SOURCE_DIR}/R-package"
+    DIRECTORY "${boxhed_kernel_SOURCE_DIR}/R-package"
     DESTINATION "${build_dir}"
     REGEX "src/*" EXCLUDE
     REGEX "R-package/configure" EXCLUDE
   )
   install(TARGETS ${rlib_target}
     LIBRARY DESTINATION "${build_dir}/R-package/src/"
     RUNTIME DESTINATION "${build_dir}/R-package/src/")
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/Sanitizer.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/Utils.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/Utils.cmake`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
   find_package(NVTX REQUIRED)
   target_include_directories(${target} PRIVATE "${NVTX_INCLUDE_DIR}")
   target_link_libraries(${target} PRIVATE "${NVTX_LIBRARY}")
   target_compile_definitions(${target} PRIVATE -DXGBOOST_USE_NVTX=1)
 endmacro()
 
 # Set CUDA related flags to target.  Must be used after code `format_gencode_flags`.
-function(xgboost_set_cuda_flags target)
+function(boxhed_kernel_set_cuda_flags target)
   find_package(OpenMP REQUIRED)
   target_link_libraries(${target} PUBLIC OpenMP::OpenMP_CXX)
 
   target_compile_options(${target} PRIVATE
     $<$<COMPILE_LANGUAGE:CUDA>:--expt-extended-lambda>
     $<$<COMPILE_LANGUAGE:CUDA>:--expt-relaxed-constexpr>
     $<$<COMPILE_LANGUAGE:CUDA>:${GEN_CODE}>
@@ -152,15 +152,15 @@
   endif (USE_DEVICE_DEBUG)
 
   if (USE_NVTX)
     enable_nvtx(${target})
   endif (USE_NVTX)
 
   target_compile_definitions(${target} PRIVATE -DXGBOOST_USE_CUDA=1 -DTHRUST_IGNORE_CUB_VERSION_CHECK=1)
-  target_include_directories(${target} PRIVATE ${xgboost_SOURCE_DIR}/cub/)
+  target_include_directories(${target} PRIVATE ${boxhed_kernel_SOURCE_DIR}/cub/)
 
   if (MSVC)
     target_compile_options(${target} PRIVATE
       $<$<COMPILE_LANGUAGE:CUDA>:-Xcompiler=/utf-8>)
   endif (MSVC)
 
   set_target_properties(${target} PROPERTIES
@@ -175,8 +175,8 @@
 
   if (USE_NCCL)
     find_package(Nccl REQUIRED)
     target_include_directories(${target} PRIVATE ${NCCL_INCLUDE_DIR})
     target_compile_definitions(${target} PRIVATE -DXGBOOST_USE_NCCL=1)
     target_link_libraries(${target} PUBLIC ${NCCL_LIBRARY})
   endif (USE_NCCL)
-endfunction(xgboost_set_cuda_flags)
+endfunction(boxhed_kernel_set_cuda_flags)
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindLibR.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindLibR.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindNVML.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindNVML.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindNVTX.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindNVTX.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/cmake/modules/FindNccl.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/cmake/modules/FindNccl.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/CMakeLists.txt` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/LICENSE` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/LICENSE`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/Makefile` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/Makefile`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/README.md` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/README.md`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/appveyor.yml` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/appveyor.yml`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Modules/FindHDFS.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Modules/FindHDFS.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Sanitizer.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/Utils.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/Utils.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/build_config.h.in` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/build_config.h.in`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/cmake/lint.cmake` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/cmake/lint.cmake`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/Doxyfile` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/Doxyfile`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/Makefile` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/Makefile`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/conf.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/conf.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/doc/parameter.md` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/doc/parameter.md`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/example/parameter.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/example/parameter.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/any.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/any.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/array_view.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/array_view.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/base.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/base.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/blockingconcurrentqueue.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/blockingconcurrentqueue.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/build_config_default.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/build_config_default.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/common.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/common.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/concurrency.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/concurrency.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/concurrentqueue.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/concurrentqueue.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/config.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/config.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/data.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/data.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/endian.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/endian.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/filesystem.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/filesystem.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/input_split_shuffle.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/input_split_shuffle.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/io.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/io.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/json.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/json.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/logging.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/logging.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/lua.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/lua.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/memory.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/memory.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/memory_io.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/memory_io.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/omp.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/omp.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/optional.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/optional.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/parameter.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/parameter.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/recordio.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/recordio.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/registry.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/registry.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/serializer.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/serializer.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/strtonum.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/strtonum.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/thread_group.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/thread_group.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/thread_local.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/thread_local.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/threadediter.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/threadediter.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/timer.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/timer.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/include/dmlc/type_traits.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/include/dmlc/type_traits.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/make/config.mk` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/make/config.mk`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/make/dmlc.mk` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/make/dmlc.mk`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/lint.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/lint.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/packages.mk` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/packages.mk`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/s390x/Dockerfile` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/s390x/Dockerfile`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/s390x/ci_build.sh` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/s390x/ci_build.sh`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/s390x/entrypoint.sh` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/s390x/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/scripts/test_script.sh` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/scripts/test_script.sh`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/config.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/config.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/basic_row_iter.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/basic_row_iter.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/csv_parser.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/csv_parser.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/disk_row_iter.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/disk_row_iter.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/libfm_parser.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/libfm_parser.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/libsvm_parser.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/libsvm_parser.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/parser.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/parser.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/row_block.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/row_block.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data/text_parser.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data/text_parser.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/data.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/data.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/azure_filesys.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/azure_filesys.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/azure_filesys.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/azure_filesys.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/cached_input_split.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/cached_input_split.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/filesys.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/filesys.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/hdfs_filesys.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/hdfs_filesys.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/hdfs_filesys.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/hdfs_filesys.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/indexed_recordio_split.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/indexed_recordio_split.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/indexed_recordio_split.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/indexed_recordio_split.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/input_split_base.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/input_split_base.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/input_split_base.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/input_split_base.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/line_split.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/line_split.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/line_split.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/line_split.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/local_filesys.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/local_filesys.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/local_filesys.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/local_filesys.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/recordio_split.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/recordio_split.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/recordio_split.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/recordio_split.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/s3_filesys.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/s3_filesys.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/s3_filesys.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/s3_filesys.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/single_file_split.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/single_file_split.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/single_threaded_input_split.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/single_threaded_input_split.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/threaded_input_split.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/threaded_input_split.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io/uri_spec.h` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io/uri_spec.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/io.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/io.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/src/recordio.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/src/recordio.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/README.md` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/README.md`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/csv_parser_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/csv_parser_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/dataiter_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/dataiter_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/dmlc_test.mk` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/dmlc_test.mk`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/filesys_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/filesys_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/iostream_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/iostream_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/libfm_parser_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/libfm_parser_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/libsvm_parser_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/libsvm_parser_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/parameter_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/parameter_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/recordio_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/recordio_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/registry_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/registry_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/split_read_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/split_read_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/split_repeat_read_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/split_repeat_read_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/split_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/split_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/stream_read_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/stream_read_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/strtonum_test.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/strtonum_test.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/CMakeLists.txt` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/sample.rec` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/sample.rec`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_any.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_any.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_config.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_config.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_env.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_env.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_inputsplit.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_inputsplit.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_json.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_json.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_lockfree.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_lockfree.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_optional.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_optional.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_param.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_param.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_parser.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_parser.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_serializer.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_serializer.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_tempdir.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_tempdir.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_thread_group.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_thread_group.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_threaditer.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_threaditer.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/test/unittest/unittest_threaditer_exc_handling.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/test/unittest/unittest_threaditer_exc_handling.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/README.md` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/README.md`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/kubernetes.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/kubernetes.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/launcher.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/launcher.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/local.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/local.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/mesos.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/mesos.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/mpi.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/mpi.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/opts.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/opts.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/sge.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/sge.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/slurm.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/slurm.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/ssh.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/ssh.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/submit.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/submit.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/tracker.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/yarn.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/dmlc_tracker/yarn.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/pom.xml` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/pom.xml`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/ApplicationMaster.java` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/ApplicationMaster.java`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/Client.java` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/Client.java`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/TaskRecord.java` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/TaskRecord.java`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/windows/dmlc/dmlc.vcxproj` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/windows/dmlc/dmlc.vcxproj`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/dmlc-core/windows/dmlc.sln` & `boxhed_kernel-2.0.2/boxhed_kernel/dmlc-core/windows/dmlc.sln`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/base.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/base.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*!
  * Copyright (c) 2015 by Contributors
  * \file base.h
- * \brief defines configuration macros of xgboost.
+ * \brief defines configuration macros of boxhed_kernel.
  */
 #ifndef XGBOOST_BASE_H_
 #define XGBOOST_BASE_H_
 
 #include <dmlc/base.h>
 #include <dmlc/omp.h>
 #include <cmath>
@@ -102,16 +102,16 @@
 #elif defined(__GNUC__)
 // Enable __builtin_prefetch for GCC
 #define XGBOOST_BUILTIN_PREFETCH_PRESENT
 #endif  // GUARDS
 
 #endif  // !defined(XGBOOST_MM_PREFETCH_PRESENT) && !defined()
 
-/*! \brief namespace of xgboost*/
-namespace xgboost {
+/*! \brief namespace of boxhed_kernel*/
+namespace boxhed_kernel {
 
 /*! \brief unsigned integer type used for feature index. */
 using bst_uint = uint32_t;  // NOLINT
 /*! \brief integer type. */
 using bst_int = int32_t;    // NOLINT
 /*! \brief unsigned long integers */
 using bst_ulong = uint64_t;  // NOLINT
@@ -277,10 +277,10 @@
  */
 #if DMLC_USE_CXX11 && defined(__GNUC__) && !defined(__clang_version__)
 #if __GNUC__ == 4 && __GNUC_MINOR__ < 8
 #define override
 #define final
 #endif  // __GNUC__ == 4 && __GNUC_MINOR__ < 8
 #endif  // DMLC_USE_CXX11 && defined(__GNUC__) && !defined(__clang_version__)
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_BASE_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/c_api.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/c_api.h`

 * *Files 2% similar despite different names*

```diff
@@ -495,15 +495,15 @@
  *  - feature_weights
  *
  * \param handle An instance of data matrix
  * \param field  Feild name
  * \param data   Pointer to consecutive memory storing data.
  * \param size   Size of the data, this is relative to size of type.  (Meaning NOT number
  *               of bytes.)
- * \param type   Indicator of data type.  This is defined in xgboost::DataType enum class.
+ * \param type   Indicator of data type.  This is defined in boxhed_kernel::DataType enum class.
  *
  *    float    = 1
  *    double   = 2
  *    uint32_t = 3
  *    uint64_t = 4
  *
  * \return 0 when success, -1 when failure happens
@@ -560,15 +560,15 @@
  * \param out The output of number of columns
  * \return 0 when success, -1 when failure happens
  */
 XGB_DLL int XGDMatrixNumCol(DMatrixHandle handle,
                             bst_ulong *out);
 // --- start XGBoost class
 /*!
- * \brief create xgboost learner
+ * \brief create boxhed_kernel learner
  * \param dmats matrices that are set to be cached
  * \param len length of dmats
  * \param out handle to the result booster
  * \return 0 when success, -1 when failure happens
  */
 XGB_DLL int XGBoosterCreate(const DMatrixHandle dmats[],
                             bst_ulong len,
@@ -638,15 +638,15 @@
  */
 XGB_DLL int XGBoosterBoostOneIter(BoosterHandle handle,
                                   DMatrixHandle dtrain,
                                   float *grad,
                                   float *hess,
                                   bst_ulong len);
 /*!
- * \brief get evaluation statistics for xgboost
+ * \brief get evaluation statistics for boxhed_kernel
  * \param handle handle
  * \param iter current iteration rounds
  * \param dmats pointers to data to be evaluated
  * \param evnames pointers to names of each data
  * \param len length of dmats
  * \param out_result the string containing evaluation statistics
  * \return 0 when success, -1 when failure happens
@@ -735,15 +735,15 @@
  * \return 0 when success, -1 when failure happens
  */
 XGB_DLL int XGBoosterLoadModelFromBuffer(BoosterHandle handle,
                                          const void *buf,
                                          bst_ulong len);
 /*!
  * \brief save model into binary raw bytes, return header of the array
- * user must copy the result out, before next xgboost call
+ * user must copy the result out, before next boxhed_kernel call
  * \param handle handle
  * \param out_len the argument to hold the output length
  * \param out_dptr the argument to hold the output data pointer
  * \return 0 when success, -1 when failure happens
  */
 XGB_DLL int XGBoosterGetModelRaw(BoosterHandle handle, bst_ulong *out_len,
                                  const char **out_dptr);
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/data.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/data.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 /*!
  * Copyright (c) 2015 by Contributors
  * \file data.h
- * \brief The input data structure of xgboost.
+ * \brief The input data structure of boxhed_kernel.
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_DATA_H_
 #define XGBOOST_DATA_H_
 
 #include <dmlc/base.h>
 #include <dmlc/data.h>
 #include <dmlc/serializer.h>
-#include <xgboost/base.h>
-#include <xgboost/span.h>
-#include <xgboost/host_device_vector.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/span.h>
+#include <boxhed_kernel/host_device_vector.h>
 
 #include <memory>
 #include <numeric>
 #include <algorithm>
 #include <string>
 #include <utility>
 #include <vector>
 
-namespace xgboost {
+namespace boxhed_kernel {
 // forward declare dmatrix.
 class DMatrix;
 
-/*! \brief data type accepted by xgboost interface */
+/*! \brief data type accepted by boxhed_kernel interface */
 enum class DataType : uint8_t {
   kFloat32 = 1,
   kDouble = 2,
   kUInt32 = 3,
   kUInt64 = 4,
   kStr = 5
 };
@@ -60,15 +60,15 @@
    *  needed when the learning task is ranking.
    */
   std::vector<bst_group_t> group_ptr_;  // NOLINT
   /*! \brief weights of each instance, optional */
   HostDeviceVector<bst_float> weights_;  // NOLINT
   /*!
    * \brief initialized margins,
-   * if specified, xgboost will start from this init margin
+   * if specified, boxhed_kernel will start from this init margin
    * can be used to specify initial prediction to boost from.
    */
   HostDeviceVector<bst_float> base_margin_;  // NOLINT
   /*!
    * \brief lower bound of the label, to be used for survival analysis (censored regression)
    */
   HostDeviceVector<bst_float> labels_lower_bound_;  // NOLINT
@@ -588,29 +588,29 @@
   return GetSortedColumnBatches();
 }
 
 template<>
 inline BatchSet<EllpackPage> DMatrix::GetBatches(const BatchParam& param) {
   return GetEllpackBatches(param);
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 namespace dmlc {
-DMLC_DECLARE_TRAITS(is_pod, xgboost::Entry, true);
+DMLC_DECLARE_TRAITS(is_pod, boxhed_kernel::Entry, true);
 
 namespace serializer {
 
 template <>
-struct Handler<xgboost::Entry> {
-  inline static void Write(Stream* strm, const xgboost::Entry& data) {
+struct Handler<boxhed_kernel::Entry> {
+  inline static void Write(Stream* strm, const boxhed_kernel::Entry& data) {
     strm->Write(data.index);
     strm->Write(data.fvalue);
   }
 
-  inline static bool Read(Stream* strm, xgboost::Entry* data) {
+  inline static bool Read(Stream* strm, boxhed_kernel::Entry* data) {
     return strm->Read(&data->index) && strm->Read(&data->fvalue);
   }
 };
 
 }  // namespace serializer
 }  // namespace dmlc
 #endif  // XGBOOST_DATA_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/feature_map.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/feature_map.h`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
  * \file feature_map.h
  * \brief Feature map data structure to help visualization and model dump.
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_FEATURE_MAP_H_
 #define XGBOOST_FEATURE_MAP_H_
 
-#include <xgboost/logging.h>
+#include <boxhed_kernel/logging.h>
 
 #include <vector>
 #include <string>
 #include <cstring>
 #include <iostream>
 
-namespace xgboost {
+namespace boxhed_kernel {
 /*!
  * \brief Feature map data structure to help text model dump.
  * TODO(tqchen) consider make it even more lightweight.
  */
 class FeatureMap {
  public:
   /*! \brief type of feature maps */
@@ -86,9 +86,9 @@
     return kIndicator;
   }
   /*! \brief name of the feature */
   std::vector<std::string> names_;
   /*! \brief type of the feature */
   std::vector<Type> types_;
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_FEATURE_MAP_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/gbm.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/gbm.h`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,27 @@
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_GBM_H_
 #define XGBOOST_GBM_H_
 
 #include <dmlc/registry.h>
 #include <dmlc/any.h>
-#include <xgboost/base.h>
-#include <xgboost/data.h>
-#include <xgboost/host_device_vector.h>
-#include <xgboost/model.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/host_device_vector.h>
+#include <boxhed_kernel/model.h>
 
 #include <vector>
 #include <utility>
 #include <string>
 #include <functional>
 #include <unordered_map>
 #include <memory>
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 class Json;
 class FeatureMap;
 class ObjFunction;
 
 struct GenericParameter;
 struct LearnerModelParam;
@@ -213,13 +213,13 @@
  * .describe("Boosting tree ensembles.")
  * .set_body([]() {
  *     return new GradientBooster<TStats>();
  *   });
  * \endcode
  */
 #define XGBOOST_REGISTER_GBM(UniqueId, Name)                            \
-  static DMLC_ATTRIBUTE_UNUSED ::xgboost::GradientBoosterReg &          \
+  static DMLC_ATTRIBUTE_UNUSED ::boxhed_kernel::GradientBoosterReg &          \
   __make_ ## GradientBoosterReg ## _ ## UniqueId ## __ =                \
-      ::dmlc::Registry< ::xgboost::GradientBoosterReg>::Get()->__REGISTER__(Name)
+      ::dmlc::Registry< ::boxhed_kernel::GradientBoosterReg>::Get()->__REGISTER__(Name)
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_GBM_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/generic_parameters.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/generic_parameters.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 /*!
  * Copyright 2014-2019 by Contributors
  * \file generic_parameters.h
  */
 #ifndef XGBOOST_GENERIC_PARAMETERS_H_
 #define XGBOOST_GENERIC_PARAMETERS_H_
 
-#include <xgboost/logging.h>
-#include <xgboost/parameter.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/parameter.h>
 
 #include <string>
 
-namespace xgboost {
+namespace boxhed_kernel {
 struct GenericParameter : public XGBoostParameter<GenericParameter> {
   // Constant representing the device ID of CPU.
   static int32_t constexpr kCpuId = -1;
   static int64_t constexpr kDefaultSeed = 0;
 
  public:
   // stored random seed
@@ -84,10 +84,10 @@
 "\n\tThis can be done using Dask or Spark.  See documentation for details.");
   }
 
  private:
   // number of devices to use (deprecated).
   int n_gpus {0};  // NOLINT
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_GENERIC_PARAMETERS_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/host_device_vector.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/host_device_vector.h`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  *                        (assuming 'DevicePointer' is not called in between)
  * DevicePointer but data on CPU  --> this causes a cudaMemcpy to be issued internally.
  *                        subsequent calls to DevicePointer, will NOT incur this penalty.
  *                        (assuming 'HostVector' is not called in between)
  * DevicePointer and data on GPU  --> no problems, the device ptr
  *                        will be returned immediately.
  *
- * What if xgboost is compiled without CUDA?<br/>
+ * What if boxhed_kernel is compiled without CUDA?<br/>
  * In that case, there's a special implementation which always falls-back to
  * working with std::vector. This logic can be found in host_device_vector.cc
  *
  * Why not consider CUDA unified memory?<br/>
  * We did consider. However, it poses complications if we need to support both
  * compiling with and without CUDA toolkit. It was easier to have
  * 'HostDeviceVector' with a special-case implementation in host_device_vector.cc
@@ -51,15 +51,15 @@
 
 #include <initializer_list>
 #include <vector>
 #include <type_traits>
 
 #include "span.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 #ifdef __CUDACC__
 // Sets a function to call instead of cudaSetDevice();
 // only added for testing
 void SetCudaSetDeviceHandler(void (*handler)(int));
 #endif  // __CUDACC__
 
@@ -138,10 +138,10 @@
 
   using value_type = T;  // NOLINT
 
  private:
   HostDeviceVectorImpl<T>* impl_;
 };
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_HOST_DEVICE_VECTOR_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/intrusive_ptr.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/intrusive_ptr.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef XGBOOST_INTRUSIVE_PTR_H_
 #define XGBOOST_INTRUSIVE_PTR_H_
 
 #include <atomic>
 #include <cinttypes>
 #include <functional>
 
-namespace xgboost {
+namespace boxhed_kernel {
 /*!
  * \brief Helper class for embedding reference counting into client objects.  See
  *        https://www.boost.org/doc/libs/1_74_0/doc/html/atomic/usage_examples.html for
  *        discussions of memory order.
  */
 class IntrusivePtrCell {
  private:
@@ -197,20 +197,20 @@
 
 template <class E, class T, class Y>
 std::basic_ostream<E, T> &operator<<(std::basic_ostream<E, T> &os,
                                      IntrusivePtr<Y> const &p) {
   os << p.get();
   return os;
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 namespace std {
 template <class T>
-void swap(xgboost::IntrusivePtr<T> &x,  // NOLINT
-          xgboost::IntrusivePtr<T> &y) noexcept {
+void swap(boxhed_kernel::IntrusivePtr<T> &x,  // NOLINT
+          boxhed_kernel::IntrusivePtr<T> &y) noexcept {
   x.swap(y);
 }
 
 template <typename T>
-struct hash<xgboost::IntrusivePtr<T>> : public xgboost::IntrusivePtr<T>::Hash {};
+struct hash<boxhed_kernel::IntrusivePtr<T>> : public boxhed_kernel::IntrusivePtr<T>::Hash {};
 }      // namespace std
 #endif  // XGBOOST_INTRUSIVE_PTR_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/json.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/json.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 /*!
  * Copyright (c) by XGBoost Contributors 2019-2020
  */
 #ifndef XGBOOST_JSON_H_
 #define XGBOOST_JSON_H_
 
-#include <xgboost/logging.h>
-#include <xgboost/parameter.h>
-#include <xgboost/intrusive_ptr.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/parameter.h>
+#include <boxhed_kernel/intrusive_ptr.h>
 
 #include <map>
 #include <memory>
 #include <vector>
 #include <functional>
 #include <utility>
 #include <string>
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 class Json;
 class JsonReader;
 class JsonWriter;
 
 class Value {
  private:
   mutable class IntrusivePtrCell ref_;
   friend IntrusivePtrCell &
-  IntrusivePtrRefCount(xgboost::Value const *t) noexcept {
+  IntrusivePtrRefCount(boxhed_kernel::Value const *t) noexcept {
     return t->ref_;
   }
 
  public:
   /*!\brief Simplified implementation of LLVM RTTI. */
   enum class ValueKind {
     kString,
@@ -572,9 +572,9 @@
   auto const& j_param = get<Object const>(obj);
   std::map<std::string, std::string> m;
   for (auto const& kv : j_param) {
     m[kv.first] = get<String const>(kv.second);
   }
   param->UpdateAllowUnknown(m);
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_JSON_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/json_io.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/json_io.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*!
  * Copyright (c) by Contributors 2019
  */
 #ifndef XGBOOST_JSON_IO_H_
 #define XGBOOST_JSON_IO_H_
-#include <xgboost/json.h>
-#include <xgboost/base.h>
+#include <boxhed_kernel/json.h>
+#include <boxhed_kernel/base.h>
 
 #include <vector>
 #include <memory>
 #include <string>
 #include <utility>
 #include <map>
 #include <limits>
 #include <sstream>
 #include <locale>
 #include <cinttypes>
 
-namespace xgboost {
+namespace boxhed_kernel {
 /*
  * \brief A json reader, currently error checking and utf-8 is not fully supported.
  */
 class JsonReader {
  protected:
   size_t constexpr static kMaxNumLength =
       std::numeric_limits<double>::max_digits10 + 1;
@@ -130,10 +130,10 @@
   virtual void Visit(JsonObject const* obj);
   virtual void Visit(JsonNumber const* num);
   virtual void Visit(JsonInteger const* num);
   virtual void Visit(JsonNull   const* null);
   virtual void Visit(JsonString const* str);
   virtual void Visit(JsonBoolean const* boolean);
 };
-}      // namespace xgboost
+}      // namespace boxhed_kernel
 
 #endif  // XGBOOST_JSON_IO_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/learner.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/learner.h`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
  *  This is the user facing XGBoost training module.
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_LEARNER_H_
 #define XGBOOST_LEARNER_H_
 
 #include <dmlc/any.h>
-#include <xgboost/base.h>
-#include <xgboost/feature_map.h>
-#include <xgboost/predictor.h>
-#include <xgboost/generic_parameters.h>
-#include <xgboost/host_device_vector.h>
-#include <xgboost/model.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/feature_map.h>
+#include <boxhed_kernel/predictor.h>
+#include <boxhed_kernel/generic_parameters.h>
+#include <boxhed_kernel/host_device_vector.h>
+#include <boxhed_kernel/model.h>
 
 #include <utility>
 #include <map>
 #include <memory>
 #include <string>
 #include <vector>
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 class Metric;
 class GradientBooster;
 class ObjFunction;
 class DMatrix;
 class Json;
 
@@ -44,15 +44,15 @@
   std::vector<GradientPair> tmp_gpair;
   PredictionCacheEntry prediction_entry;
 };
 
 
 /*!
  * \brief Learner class that does training and prediction.
- *  This is the user facing module of xgboost training.
+ *  This is the user facing module of boxhed_kernel training.
  *  The Load/Save function corresponds to the model used in python/R.
  *  \code
  *
  *  std::unique_ptr<Learner> learner(new Learner::Create(cache_mats));
  *  learner.Configure(configs);
  *
  *  for (int iter = 0; iter < max_iter; ++iter) {
@@ -261,9 +261,9 @@
   // As the old `LearnerModelParamLegacy` is still used by binary IO, we keep
   // this one as an immutable copy.
   LearnerModelParam(LearnerModelParamLegacy const& user_param, float base_margin);
   /* \brief Whether this parameter is initialized with LearnerModelParamLegacy. */
   bool Initialized() const { return num_feature != 0; }
 };
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_LEARNER_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/logging.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/logging.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 /*!
  * Copyright (c) 2015-2019 by Contributors
  * \file logging.h
  *
- * \brief defines console logging options for xgboost.  Use to enforce unified print
+ * \brief defines console logging options for boxhed_kernel.  Use to enforce unified print
  *  behavior.
  */
 #ifndef XGBOOST_LOGGING_H_
 #define XGBOOST_LOGGING_H_
 
 #include <dmlc/logging.h>
 #include <dmlc/thread_local.h>
 
-#include <xgboost/base.h>
-#include <xgboost/parameter.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/parameter.h>
 
 #include <sstream>
 #include <map>
 #include <string>
 #include <utility>
 #include <vector>
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 class BaseLogger {
  public:
   BaseLogger() {
 #if XGBOOST_LOG_WITH_TIME
     log_stream_ << "[" << dmlc::DateLogger().HumanDate() << "] ";
 #endif  // XGBOOST_LOG_WITH_TIME
@@ -114,52 +114,52 @@
 using LogCallbackRegistryStore = dmlc::ThreadLocalStore<LogCallbackRegistry>;
 
 // Redefines LOG_WARNING for controling verbosity
 #if defined(LOG_WARNING)
 #undef  LOG_WARNING
 #endif  // defined(LOG_WARNING)
 #define LOG_WARNING                                                            \
-  if (::xgboost::ConsoleLogger::ShouldLog(                                     \
-          ::xgboost::ConsoleLogger::LV::kWarning))                             \
-  ::xgboost::ConsoleLogger(__FILE__, __LINE__,                                 \
-                           ::xgboost::ConsoleLogger::LogVerbosity::kWarning)
+  if (::boxhed_kernel::ConsoleLogger::ShouldLog(                                     \
+          ::boxhed_kernel::ConsoleLogger::LV::kWarning))                             \
+  ::boxhed_kernel::ConsoleLogger(__FILE__, __LINE__,                                 \
+                           ::boxhed_kernel::ConsoleLogger::LogVerbosity::kWarning)
 
 // Redefines LOG_INFO for controling verbosity
 #if defined(LOG_INFO)
 #undef  LOG_INFO
 #endif  // defined(LOG_INFO)
 #define LOG_INFO                                                               \
-  if (::xgboost::ConsoleLogger::ShouldLog(                                     \
-          ::xgboost::ConsoleLogger::LV::kInfo))                                \
-  ::xgboost::ConsoleLogger(__FILE__, __LINE__,                                 \
-                           ::xgboost::ConsoleLogger::LogVerbosity::kInfo)
+  if (::boxhed_kernel::ConsoleLogger::ShouldLog(                                     \
+          ::boxhed_kernel::ConsoleLogger::LV::kInfo))                                \
+  ::boxhed_kernel::ConsoleLogger(__FILE__, __LINE__,                                 \
+                           ::boxhed_kernel::ConsoleLogger::LogVerbosity::kInfo)
 
 #if defined(LOG_DEBUG)
 #undef LOG_DEBUG
 #endif  // defined(LOG_DEBUG)
 #define LOG_DEBUG                                                              \
-  if (::xgboost::ConsoleLogger::ShouldLog(                                     \
-          ::xgboost::ConsoleLogger::LV::kDebug))                               \
-  ::xgboost::ConsoleLogger(__FILE__, __LINE__,                                 \
-                           ::xgboost::ConsoleLogger::LogVerbosity::kDebug)
+  if (::boxhed_kernel::ConsoleLogger::ShouldLog(                                     \
+          ::boxhed_kernel::ConsoleLogger::LV::kDebug))                               \
+  ::boxhed_kernel::ConsoleLogger(__FILE__, __LINE__,                                 \
+                           ::boxhed_kernel::ConsoleLogger::LogVerbosity::kDebug)
 
 // redefines the logging macro if not existed
 #ifndef LOG
 #define LOG(severity) LOG_##severity.stream()
 #endif  // LOG
 
 // Enable LOG(CONSOLE) for print messages to console.
-#define LOG_CONSOLE ::xgboost::ConsoleLogger(           \
-    ::xgboost::ConsoleLogger::LogVerbosity::kIgnore)
+#define LOG_CONSOLE ::boxhed_kernel::ConsoleLogger(           \
+    ::boxhed_kernel::ConsoleLogger::LogVerbosity::kIgnore)
 // Enable LOG(TRACKER) for print messages to tracker
-#define LOG_TRACKER ::xgboost::TrackerLogger()
+#define LOG_TRACKER ::boxhed_kernel::TrackerLogger()
 
 #if defined(CHECK)
 #undef CHECK
 #define CHECK(cond)                                     \
   if (XGBOOST_EXPECT(!(cond), false))                   \
     dmlc::LogMessageFatal(__FILE__, __LINE__).stream()  \
         << "Check failed: " #cond << ": "
 #endif  // defined(CHECK)
 
-}  // namespace xgboost.
+}  // namespace boxhed_kernel.
 #endif  // XGBOOST_LOGGING_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/metric.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/metric.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 /*!
  * Copyright 2014 by Contributors
  * \file metric.h
- * \brief interface of evaluation metric function supported in xgboost.
+ * \brief interface of evaluation metric function supported in boxhed_kernel.
  * \author Tianqi Chen, Kailong Chen
  */
 #ifndef XGBOOST_METRIC_H_
 #define XGBOOST_METRIC_H_
 
 #include <dmlc/registry.h>
-#include <xgboost/model.h>
-#include <xgboost/generic_parameters.h>
-#include <xgboost/data.h>
-#include <xgboost/base.h>
-#include <xgboost/host_device_vector.h>
+#include <boxhed_kernel/model.h>
+#include <boxhed_kernel/generic_parameters.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/host_device_vector.h>
 
 #include <vector>
 #include <string>
 #include <functional>
 #include <utility>
 
-namespace xgboost {
+namespace boxhed_kernel {
 /*!
  * \brief interface of evaluation metric used to evaluate model performance.
  *  This has nothing to do with training, but merely act as evaluation purpose.
  */
 class Metric : public Configurable {
  protected:
   GenericParameter const* tparam_;
@@ -96,11 +96,11 @@
  * .set_body([](const char* param) {
  *     int at_k = atoi(param);
  *     return new NDCG(at_k);
  *   });
  * \endcode
  */
 #define XGBOOST_REGISTER_METRIC(UniqueId, Name)                         \
-  ::xgboost::MetricReg&  __make_ ## MetricReg ## _ ## UniqueId ## __ =  \
-      ::dmlc::Registry< ::xgboost::MetricReg>::Get()->__REGISTER__(Name)
-}  // namespace xgboost
+  ::boxhed_kernel::MetricReg&  __make_ ## MetricReg ## _ ## UniqueId ## __ =  \
+      ::dmlc::Registry< ::boxhed_kernel::MetricReg>::Get()->__REGISTER__(Name)
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_METRIC_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/model.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/model.h`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef XGBOOST_MODEL_H_
 #define XGBOOST_MODEL_H_
 
 namespace dmlc {
 class Stream;
 }  // namespace dmlc
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 class Json;
 
 struct Model {
   virtual ~Model() = default;
   /*!
    * \brief load the model from a json object
@@ -37,10 +37,10 @@
   virtual void LoadConfig(Json const& in) = 0;
   /*!
    * \brief Save configuration to JSON object
    * \param out pointer to output JSON object
    */
   virtual void SaveConfig(Json* out) const = 0;
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_MODEL_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/objective.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/objective.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 /*!
  * Copyright 2014-2019 by Contributors
  * \file objective.h
- * \brief interface of objective function used by xgboost.
+ * \brief interface of objective function used by boxhed_kernel.
  * \author Tianqi Chen, Kailong Chen
  */
 #ifndef XGBOOST_OBJECTIVE_H_
 #define XGBOOST_OBJECTIVE_H_
 
 #include <dmlc/registry.h>
-#include <xgboost/base.h>
-#include <xgboost/data.h>
-#include <xgboost/model.h>
-#include <xgboost/generic_parameters.h>
-#include <xgboost/host_device_vector.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/model.h>
+#include <boxhed_kernel/generic_parameters.h>
+#include <boxhed_kernel/host_device_vector.h>
 
 #include <vector>
 #include <utility>
 #include <string>
 #include <functional>
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 /*! \brief interface of objective function */
 class ObjFunction : public Configurable {
  protected:
   GenericParameter const* tparam_;
 
  public:
@@ -97,12 +97,12 @@
  * .describe("Linear regression objective")
  * .set_body([]() {
  *     return new RegLossObj(LossType::kLinearSquare);
  *   });
  * \endcode
  */
 #define XGBOOST_REGISTER_OBJECTIVE(UniqueId, Name)                      \
-  static DMLC_ATTRIBUTE_UNUSED ::xgboost::ObjFunctionReg &              \
+  static DMLC_ATTRIBUTE_UNUSED ::boxhed_kernel::ObjFunctionReg &              \
   __make_ ## ObjFunctionReg ## _ ## UniqueId ## __ =                    \
-      ::dmlc::Registry< ::xgboost::ObjFunctionReg>::Get()->__REGISTER__(Name)
-}  // namespace xgboost
+      ::dmlc::Registry< ::boxhed_kernel::ObjFunctionReg>::Get()->__REGISTER__(Name)
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_OBJECTIVE_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/parameter.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/parameter.h`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
  * \author Hyunsu Philip Cho
  */
 
 #ifndef XGBOOST_PARAMETER_H_
 #define XGBOOST_PARAMETER_H_
 
 #include <dmlc/parameter.h>
-#include <xgboost/base.h>
+#include <boxhed_kernel/base.h>
 #include <string>
 #include <type_traits>
 
 /*!
  * \brief Specialization of FieldEntry for enum class (backed by int)
  *
  * Use this macro to use C++11 enum class as DMLC parameters
@@ -75,15 +75,15 @@
   inline void Init(const std::string &key, void *head, EnumClass& ref) {  /* NOLINT */  \
     Super::Init(key, head, *reinterpret_cast<int*>(&ref));  \
   }  \
 };  \
 }  /* namespace parameter */  \
 }  /* namespace dmlc */
 
-namespace xgboost {
+namespace boxhed_kernel {
 template <typename Type>
 struct XGBoostParameter : public dmlc::Parameter<Type> {
  protected:
   bool initialised_ {false};
 
  public:
   template <typename Container>
@@ -97,10 +97,10 @@
       }
       initialised_ = true;
       return unknown;
     }
   }
   bool GetInitialised() const { return static_cast<bool>(this->initialised_); }
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_PARAMETER_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/predictor.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/predictor.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 /*!
  * Copyright 2017-2020 by Contributors
  * \file predictor.h
  * \brief Interface of predictor,
  *  performs predictions for a gradient booster.
  */
 #pragma once
-#include <xgboost/base.h>
-#include <xgboost/data.h>
-#include <xgboost/generic_parameters.h>
-#include <xgboost/host_device_vector.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/generic_parameters.h>
+#include <boxhed_kernel/host_device_vector.h>
 
 #include <functional>
 #include <memory>
 #include <string>
 #include <unordered_map>
 #include <utility>
 #include <vector>
 #include <mutex>
 
 // Forward declarations
-namespace xgboost {
+namespace boxhed_kernel {
 class TreeUpdater;
 namespace gbm {
 struct GBTreeModel;
 }  // namespace gbm
 }
 
-namespace xgboost {
+namespace boxhed_kernel {
 /**
  * \struct  PredictionCacheEntry
  *
  * \brief Contains pointer to input matrix and associated cached predictions.
  */
 struct PredictionCacheEntry {
   // A storage for caching prediction values
@@ -227,11 +227,11 @@
  * \brief Registry entry for predictor.
  */
 struct PredictorReg
     : public dmlc::FunctionRegEntryBase<
   PredictorReg, std::function<Predictor*(GenericParameter const*)>> {};
 
 #define XGBOOST_REGISTER_PREDICTOR(UniqueId, Name)      \
-  static DMLC_ATTRIBUTE_UNUSED ::xgboost::PredictorReg& \
+  static DMLC_ATTRIBUTE_UNUSED ::boxhed_kernel::PredictorReg& \
       __make_##PredictorReg##_##UniqueId##__ =          \
-          ::dmlc::Registry<::xgboost::PredictorReg>::Get()->__REGISTER__(Name)
-}  // namespace xgboost
+          ::dmlc::Registry<::boxhed_kernel::PredictorReg>::Get()->__REGISTER__(Name)
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/span.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/span.h`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  */
 
 #ifndef XGBOOST_SPAN_H_
 #define XGBOOST_SPAN_H_
 
-#include <xgboost/base.h>
-#include <xgboost/logging.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/logging.h>
 
 #include <cinttypes>          // size_t
 #include <limits>             // numeric_limits
 #include <iterator>
 #include <type_traits>
 #include <cstdio>
 
@@ -64,15 +64,15 @@
 
 #else
 
 #define __span_noexcept noexcept
 
 #endif  // defined(_MSC_VER) && _MSC_VER < 1910
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 // Usual logging facility is not available inside device code.
 // assert is not supported in mac as of CUDA 10.0
 #define KERNEL_CHECK(cond)                                                     \
   do {                                                                         \
     if (!(cond)) {                                                             \
@@ -90,25 +90,25 @@
 #define SPAN_CHECK KERNEL_CHECK
 #elif defined(XGBOOST_STRICT_R_MODE) && XGBOOST_STRICT_R_MODE == 1  // R package
 #define SPAN_CHECK CHECK  // check from dmlc
 #else  // not CUDA, not R
 #define SPAN_CHECK(cond)                                                       \
   do {                                                                         \
     if (XGBOOST_EXPECT(!(cond), false)) {                                      \
-      fprintf(stderr, "[xgboost] Condition %s failed.\n", #cond);              \
+      fprintf(stderr, "[boxhed_kernel] Condition %s failed.\n", #cond);              \
       fflush(stderr);  /* It seems stderr on Windows is beffered? */           \
       std::terminate();                                                        \
     }                                                                          \
   } while (0);
 #endif  // __CUDA_ARCH__
 
 #if defined(__CUDA_ARCH__)
 #define SPAN_LT(lhs, rhs)                                                      \
   if (!((lhs) < (rhs))) {                                                      \
-    printf("[xgboost] Condition: %lu < %lu failed\n",                          \
+    printf("[boxhed_kernel] Condition: %lu < %lu failed\n",                          \
            static_cast<size_t>(lhs), static_cast<size_t>(rhs));                \
     asm("trap;");                                                              \
   }
 #else
 #define SPAN_LT(lhs, rhs) SPAN_CHECK((lhs) < (rhs))
 #endif  // defined(__CUDA_ARCH__)
 
@@ -655,15 +655,15 @@
 template <class T, std::size_t E>
 XGBOOST_DEVICE auto as_writable_bytes(Span<T, E> s) __span_noexcept ->  // NOLINT
     Span<byte, detail::ExtentAsBytesValue<T, E>::value> {
   return {reinterpret_cast<byte*>(s.data()), s.size_bytes()};
 }
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #if defined(_MSC_VER) &&_MSC_VER < 1910
 #undef constexpr
 #pragma pop_macro("constexpr")
 #undef __span_noexcept
 #endif  // _MSC_VER < 1910
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/tree_model.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/tree_model.h`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
  */
 #ifndef XGBOOST_TREE_MODEL_H_
 #define XGBOOST_TREE_MODEL_H_
 
 #include <dmlc/io.h>
 #include <dmlc/parameter.h>
 
-#include <xgboost/base.h>
-#include <xgboost/data.h>
-#include <xgboost/logging.h>
-#include <xgboost/feature_map.h>
-#include <xgboost/model.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/feature_map.h>
+#include <boxhed_kernel/model.h>
 
 #include <limits>
 #include <vector>
 #include <string>
 #include <cstring>
 #include <algorithm>
 #include <tuple>
 #include <stack>
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 struct PathElement;  // forward declaration
 
 class Json;
 // FIXME(trivialfis): Once binary IO is gone, make this parameter internal as it should
 // not be configured by users.
 /*! \brief meta parameters of the tree */
@@ -122,15 +122,15 @@
     dmlc::ByteSwap(&x.leaf_child_cnt, sizeof(x.leaf_child_cnt), 1);
     return x;
   }
 };
 
 /*!
  * \brief define regression tree to be the most common tree model.
- *  This is the data structure used in xgboost's major tree models.
+ *  This is the data structure used in boxhed_kernel's major tree models.
  */
 class RegTree : public Model {
  public:
   using SplitCondT = bst_float;
   static constexpr bst_node_t kInvalidNodeId {-1};
   static constexpr uint32_t kDeletedNodeMarker = std::numeric_limits<uint32_t>::max();
   static constexpr bst_node_t kRoot { 0 };
@@ -753,9 +753,9 @@
     // 35% speed up due to reduced miss branch predictions
     // The following expression returns the left child if (fvalue < split_cond);
     // the right child otherwise.
     return (*this)[pid].LeftChild() + !(fvalue < (*this)[pid].SplitCond());
   }
 }
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_TREE_MODEL_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/include/xgboost/tree_updater.h` & `boxhed_kernel-2.0.2/boxhed_kernel/include/boxhed_kernel/tree_updater.h`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,27 @@
  *   Updating a collection of trees given the information.
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_TREE_UPDATER_H_
 #define XGBOOST_TREE_UPDATER_H_
 
 #include <dmlc/registry.h>
-#include <xgboost/base.h>
-#include <xgboost/data.h>
-#include <xgboost/tree_model.h>
-#include <xgboost/generic_parameters.h>
-#include <xgboost/host_device_vector.h>
-#include <xgboost/model.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/tree_model.h>
+#include <boxhed_kernel/generic_parameters.h>
+#include <boxhed_kernel/host_device_vector.h>
+#include <boxhed_kernel/model.h>
 
 #include <functional>
 #include <vector>
 #include <utility>
 #include <string>
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 class Json;
 
 /*!
  * \brief interface of tree update module, that performs update of a tree.
  */
 class TreeUpdater : public Configurable {
@@ -105,13 +105,13 @@
  * .describe("Column based tree maker.")
  * .set_body([]() {
  *     return new ColMaker<TStats>();
  *   });
  * \endcode
  */
 #define XGBOOST_REGISTER_TREE_UPDATER(UniqueId, Name)                   \
-  static DMLC_ATTRIBUTE_UNUSED ::xgboost::TreeUpdaterReg&               \
+  static DMLC_ATTRIBUTE_UNUSED ::boxhed_kernel::TreeUpdaterReg&               \
   __make_ ## TreeUpdaterReg ## _ ## UniqueId ## __ =                    \
-      ::dmlc::Registry< ::xgboost::TreeUpdaterReg>::Get()->__REGISTER__(Name)
+      ::dmlc::Registry< ::boxhed_kernel::TreeUpdaterReg>::Get()->__REGISTER__(Name)
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_TREE_UPDATER_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/plugin/CMakeLists.txt` & `boxhed_kernel-2.0.2/boxhed_kernel/plugin/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 if (PLUGIN_LZ4)
-  target_sources(objxgboost PRIVATE ${xgboost_SOURCE_DIR}/plugin/lz4/sparse_page_lz4_format.cc)
+  target_sources(objboxhed_kernel PRIVATE ${boxhed_kernel_SOURCE_DIR}/plugin/lz4/sparse_page_lz4_format.cc)
   find_path(LIBLZ4_INCLUDE_DIR lz4.h)
   find_library(LIBLZ4_LIBRARY NAMES lz4)
   message(STATUS "LIBLZ4_INCLUDE_DIR = ${LIBLZ4_INCLUDE_DIR}")
   message(STATUS "LIBLZ4_LIBRARY = ${LIBLZ4_LIBRARY}")
-  target_include_directories(objxgboost PUBLIC ${LIBLZ4_INCLUDE_DIR})
-  target_link_libraries(objxgboost PUBLIC ${LIBLZ4_LIBRARY})
+  target_include_directories(objboxhed_kernel PUBLIC ${LIBLZ4_INCLUDE_DIR})
+  target_link_libraries(objboxhed_kernel PUBLIC ${LIBLZ4_LIBRARY})
 endif (PLUGIN_LZ4)
 
 if (PLUGIN_DENSE_PARSER)
-  target_sources(objxgboost PRIVATE ${xgboost_SOURCE_DIR}/plugin/dense_parser/dense_libsvm.cc)
+  target_sources(objboxhed_kernel PRIVATE ${boxhed_kernel_SOURCE_DIR}/plugin/dense_parser/dense_libsvm.cc)
 endif (PLUGIN_DENSE_PARSER)
 
 if (PLUGIN_RMM)
   find_path(RMM_INCLUDE "rmm" HINTS "$ENV{RMM_ROOT}/include")
   if (NOT RMM_INCLUDE)
     message(FATAL_ERROR "Could not locate RMM library")
   endif ()
 
   message(STATUS "RMM: RMM_LIBRARY set to ${RMM_LIBRARY}")
   message(STATUS "RMM: RMM_INCLUDE set to ${RMM_INCLUDE}")
 
-  target_include_directories(objxgboost PUBLIC ${RMM_INCLUDE})
-  target_compile_definitions(objxgboost PUBLIC -DXGBOOST_USE_RMM=1)
+  target_include_directories(objboxhed_kernel PUBLIC ${RMM_INCLUDE})
+  target_compile_definitions(objboxhed_kernel PUBLIC -DXGBOOST_USE_RMM=1)
 endif (PLUGIN_RMM)
 
 if (PLUGIN_UPDATER_ONEAPI)
   add_library(oneapi_plugin OBJECT
-    ${xgboost_SOURCE_DIR}/plugin/updater_oneapi/regression_obj_oneapi.cc
-    ${xgboost_SOURCE_DIR}/plugin/updater_oneapi/predictor_oneapi.cc)
+    ${boxhed_kernel_SOURCE_DIR}/plugin/updater_oneapi/regression_obj_oneapi.cc
+    ${boxhed_kernel_SOURCE_DIR}/plugin/updater_oneapi/predictor_oneapi.cc)
   target_include_directories(oneapi_plugin
     PRIVATE
-    ${xgboost_SOURCE_DIR}/include
-    ${xgboost_SOURCE_DIR}/dmlc-core/include
-    ${xgboost_SOURCE_DIR}/rabit/include)
+    ${boxhed_kernel_SOURCE_DIR}/include
+    ${boxhed_kernel_SOURCE_DIR}/dmlc-core/include
+    ${boxhed_kernel_SOURCE_DIR}/rabit/include)
   target_compile_definitions(oneapi_plugin PUBLIC -DXGBOOST_USE_ONEAPI=1)
   target_link_libraries(oneapi_plugin PUBLIC -fsycl)
   set_target_properties(oneapi_plugin PROPERTIES
     COMPILE_FLAGS -fsycl
     CXX_STANDARD 14
     CXX_STANDARD_REQUIRED ON
     POSITION_INDEPENDENT_CODE ON)
   if (USE_OPENMP)
     find_package(OpenMP REQUIRED)
     target_link_libraries(oneapi_plugin PUBLIC OpenMP::OpenMP_CXX)
   endif (USE_OPENMP)
-  # Get compilation and link flags of oneapi_plugin and propagate to objxgboost
-  target_link_libraries(objxgboost PUBLIC oneapi_plugin)
-  # Add all objects of oneapi_plugin to objxgboost
-  target_sources(objxgboost INTERFACE $<TARGET_OBJECTS:oneapi_plugin>)
+  # Get compilation and link flags of oneapi_plugin and propagate to objboxhed_kernel
+  target_link_libraries(objboxhed_kernel PUBLIC oneapi_plugin)
+  # Add all objects of oneapi_plugin to objboxhed_kernel
+  target_sources(objboxhed_kernel INTERFACE $<TARGET_OBJECTS:oneapi_plugin>)
 endif (PLUGIN_UPDATER_ONEAPI)
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/plugin/README.md` & `boxhed_kernel-2.0.2/boxhed_kernel/plugin/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 XGBoost Plugins Modules
 =======================
 
-This folder contains plugin modules to xgboost that can be optionally installed.  The
-plugin system helps us to extend xgboost with additional features, and add experimental
+This folder contains plugin modules to boxhed_kernel that can be optionally installed.  The
+plugin system helps us to extend boxhed_kernel with additional features, and add experimental
 features that may not yet be ready to be included in the main project.
 
 To include a certain plugin, say ```plugin_a```, you only need to add the following line
-to `xgboost/plugin/CMakeLists.txt`
+to `boxhed_kernel/plugin/CMakeLists.txt`
 ``` cmake
 set(PLUGIN_SOURCES ${PLUGIN_SOURCES}
-    ${xgboost_SOURCE_DIR}/plugin/plugin_a.cc PARENT_SCOPE)
+    ${boxhed_kernel_SOURCE_DIR}/plugin/plugin_a.cc PARENT_SCOPE)
 ```
 along with specified source file `plugin_a.cc`.
 
 Then rebuild XGBoost with CMake.
 
 Write Your Own Plugin
 ---------------------
-You can plugin your own modules to xgboost by adding code to this folder,
+You can plugin your own modules to boxhed_kernel by adding code to this folder,
 without modification to the main code repo.
 The [example](example) folder provides an example to write a plugin.
 
 List of register functions
 --------------------------
-A plugin has to register a new functionality to xgboost to be able to use it.
+A plugin has to register a new functionality to boxhed_kernel to be able to use it.
 The register macros available to plugin writers are:
 
  - XGBOOST_REGISTER_METRIC - Register an evaluation metric
  - XGBOOST_REGISTER_GBM - Register a new gradient booster that learns through
    gradient statistics
- - XGBOOST_REGISTER_OBJECTIVE - Register a new objective function used by xgboost
+ - XGBOOST_REGISTER_OBJECTIVE - Register a new objective function used by boxhed_kernel
  - XGBOOST_REGISTER_TREE_UPDATER - Register a new tree-updater which updates
    the tree given the gradient information
 
 And from dmlc-core:
 
  - DMLC_REGISTER_PARAMETER - Register a set of parameter for a specific usecase
  - DMLC_REGISTER_DATA_PARSER - Register a data parser where the data can be
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/plugin/dense_parser/dense_libsvm.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/plugin/dense_parser/dense_libsvm.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*!
  * Copyright 2015 by Contributors
  * \file dense_libsvm.cc
  * \brief Plugin to load in libsvm, but fill all the missing entries with zeros.
  *  This plugin is mainly used for benchmark purposes and do not need to be included.
  */
-#include <xgboost/base.h>
+#include <boxhed_kernel/base.h>
 #include <dmlc/data.h>
 #include <memory>
 
 namespace dmlc {
 namespace data {
 
 template<typename IndexType>
@@ -62,15 +62,15 @@
 
  private:
   RowBlock<IndexType> out_;
   std::unique_ptr<Parser<IndexType> > parser_;
   uint32_t num_col_;
   std::vector<size_t> offset_;
   std::vector<IndexType> dense_index_;
-  std::vector<xgboost::bst_float> dense_value_;
+  std::vector<boxhed_kernel::bst_float> dense_value_;
 };
 
 template<typename IndexType, typename DType = real_t>
 Parser<IndexType> *
 CreateDenseLibSVMParser(const std::string& path,
                         const std::map<std::string, std::string>& args,
                         unsigned part_index,
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/plugin/example/custom_obj.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/plugin/example/custom_obj.cc`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /*!
  * Copyright 2015-2019 by Contributors
  * \file custom_metric.cc
- * \brief This is an example to define plugin of xgboost.
+ * \brief This is an example to define plugin of boxhed_kernel.
  *  This plugin defines the additional metric function.
  */
-#include <xgboost/base.h>
-#include <xgboost/parameter.h>
-#include <xgboost/objective.h>
-#include <xgboost/json.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/parameter.h>
+#include <boxhed_kernel/objective.h>
+#include <boxhed_kernel/json.h>
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 
 // This is a helpful data structure to define parameters
 // You do not have to use it.
 // see http://dmlc-core.readthedocs.org/en/latest/parameter.html
 // for introduction of this module.
 struct MyLogisticParam : public XGBoostParameter<MyLogisticParam> {
@@ -81,14 +81,14 @@
   }
 
  private:
   MyLogisticParam param_;
 };
 
 // Finally register the objective function.
-// After it succeeds you can try use xgboost with objective=mylogistic
+// After it succeeds you can try use boxhed_kernel with objective=mylogistic
 XGBOOST_REGISTER_OBJECTIVE(MyLogistic, "mylogistic")
 .describe("User defined logistic regression plugin")
 .set_body([]() { return new MyLogistic(); });
 
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/plugin/lz4/sparse_page_lz4_format.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/plugin/lz4/sparse_page_lz4_format.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /*!
  * Copyright (c) 2015 by Contributors
  * \file sparse_page_lz4_format.cc
  *  XGBoost Plugin to enable LZ4 compressed format on the external memory pages.
  */
 #include <dmlc/registry.h>
 
-#include <xgboost/data.h>
-#include <xgboost/logging.h>
-#include <xgboost/parameter.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/parameter.h>
 #include <lz4.h>
 #include <lz4hc.h>
 #include "../../src/data/sparse_page_writer.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 DMLC_REGISTRY_FILE_TAG(sparse_page_lz4_format);
 
 // array to help compression of decompression.
 template<typename DType>
 class CompressArray {
@@ -326,8 +326,8 @@
 XGBOOST_REGISTER_SPARSE_PAGE_FORMAT(lz4i16hc)
 .describe("Apply LZ4 binary data compression(16 bit index mode) for ext memory.")
 .set_body([]() {
     return new SparsePageLZ4Format<uint16_t>(true);
   });
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_oneapi/README.md` & `boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_oneapi/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 param['objective'] = 'reg:squarederror_oneapi'
 ```
 
 ## Dependencies
 Building the plugin requires Data Parallel C++ Compiler (https://software.intel.com/content/www/us/en/develop/tools/oneapi/components/dpc-compiler.html)
 
 ## Build
-From the command line on Linux starting from the xgboost directory:
+From the command line on Linux starting from the boxhed_kernel directory:
 
 ```bash
 $ mkdir build
 $ cd build
 $ EXPORT CXX=dpcpp && cmake .. -DPLUGIN_UPDATER_ONEAPI=ON
 $ make -j
 ```
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_oneapi/predictor_oneapi.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_oneapi/predictor_oneapi.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 /*!
  * Copyright by Contributors 2017-2020
  */
 #include <cstddef>
 #include <limits>
 #include <mutex>
 
-#include "xgboost/base.h"
-#include "xgboost/data.h"
-#include "xgboost/predictor.h"
-#include "xgboost/tree_model.h"
-#include "xgboost/tree_updater.h"
-#include "xgboost/logging.h"
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/predictor.h"
+#include "boxhed_kernel/tree_model.h"
+#include "boxhed_kernel/tree_updater.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/host_device_vector.h"
 
 #include "../../src/data/adapter.h"
 #include "../../src/common/math.h"
 #include "../../src/gbm/gbtree_model.h"
 
 #include "CL/sycl.hpp"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace predictor {
 
 DMLC_REGISTRY_FILE_TAG(predictor_oneapi);
 
 /*! \brief Element from a sparse vector */
 struct EntryOneAPI {
   /*! \brief feature index */
@@ -441,8 +441,8 @@
 
 XGBOOST_REGISTER_PREDICTOR(PredictorOneAPI, "oneapi_predictor")
 .describe("Make predictions using DPC++.")
 .set_body([](GenericParameter const* generic_param) {
             return new PredictorOneAPI(generic_param);
           });
 }  // namespace predictor
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_oneapi/regression_loss_oneapi.h` & `boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_oneapi/regression_loss_oneapi.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 /*!
  * Copyright 2017-2020 XGBoost contributors
  */
 #ifndef XGBOOST_OBJECTIVE_REGRESSION_LOSS_ONEAPI_H_
 #define XGBOOST_OBJECTIVE_REGRESSION_LOSS_ONEAPI_H_
 
 #include <dmlc/omp.h>
-#include <xgboost/logging.h>
+#include <boxhed_kernel/logging.h>
 #include <algorithm>
 
 #include "CL/sycl.hpp"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 
 /*!
  * \brief calculate the sigmoid of the input.
  * \param x input parameter
  * \return the transformed value.
  */
@@ -136,10 +136,10 @@
   }
   static const char* DefaultEvalMetric() { return "auc"; }
 
   static const char* Name() { return "binary:logitraw_oneapi"; }
 };
 
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_OBJECTIVE_REGRESSION_LOSS_ONEAPI_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/plugin/updater_oneapi/regression_obj_oneapi.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/plugin/updater_oneapi/regression_obj_oneapi.cc`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-#include <xgboost/logging.h>
-#include <xgboost/objective.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/objective.h>
 #include <cmath>
 #include <memory>
 #include <vector>
 
-#include "xgboost/host_device_vector.h"
-#include "xgboost/json.h"
-#include "xgboost/parameter.h"
-#include "xgboost/span.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/span.h"
 
 #include "../../src/common/transform.h"
 #include "../../src/common/common.h"
 #include "./regression_loss_oneapi.h"
 
 #include "CL/sycl.hpp"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 
 DMLC_REGISTRY_FILE_TAG(regression_obj_oneapi);
 
 struct RegLossParamOneAPI : public XGBoostParameter<RegLossParamOneAPI> {
   float scale_pos_weight;
   // declare parameters
@@ -175,8 +175,8 @@
 .set_body([]() { return new RegLossObjOneAPI<LogisticClassificationOneAPI>(); });
 XGBOOST_REGISTER_OBJECTIVE(LogisticRawOneAPI, LogisticRawOneAPI::Name())
 .describe("Logistic regression for classification, output score "
           "before logistic transformation with DPC++ backend.")
 .set_body([]() { return new RegLossObjOneAPI<LogisticRawOneAPI>(); });
 
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/LICENSE` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/LICENSE`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/Doxyfile` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/Doxyfile`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/Makefile` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/Makefile`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/conf.py` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/conf.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/guide.md` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/guide.md`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/index.md` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/index.md`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/doc/parameters.md` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/doc/parameters.md`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/Makefile` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/Makefile`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/basic.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/basic.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/basic.py` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/basic.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/broadcast.py` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/broadcast.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/lazy_allreduce.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/lazy_allreduce.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/guide/lazy_allreduce.py` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/guide/lazy_allreduce.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/c_api.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/c_api.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/engine.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/engine.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/io.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/io.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/rabit-inl.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/rabit-inl.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/socket.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/socket.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/internal/utils.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/internal/utils.h`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #include <cstring>
 #include <cstdio>
 #include <string>
 #include <cstdlib>
 #include <stdexcept>
 #include <vector>
 #include "dmlc/io.h"
-#include "xgboost/logging.h"
+#include "boxhed_kernel/logging.h"
 #include <cstdarg>
 
 #if !defined(__GNUC__) || defined(__FreeBSD__)
 #define fopen64 std::fopen
 #endif  // !defined(__GNUC__) || defined(__FreeBSD__)
 
 #ifdef _MSC_VER
@@ -124,15 +124,15 @@
 }
 // same with Min
 template <typename T>
 auto Max(T const& l, T const& r) {
   return l > r ? l : r;
 }
 
-// easy utils that can be directly accessed in xgboost
+// easy utils that can be directly accessed in boxhed_kernel
 /*! \brief get the beginning address of a vector */
 template<typename T>
 inline T *BeginPtr(std::vector<T> &vec) {  // NOLINT(*)
   if (vec.size() == 0) {
     return nullptr;
   } else {
     return &vec[0];
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/rabit.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/rabit.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/include/rabit/serializable.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/include/rabit/serializable.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/allreduce_base.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/allreduce_base.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/allreduce_base.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/allreduce_base.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/allreduce_mock.h` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/allreduce_mock.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/c_api.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/c_api.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/engine.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/engine.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/rabit/src/engine_mpi.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit/src/engine_mpi.cc`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/CMakeLists.txt` & `boxhed_kernel-2.0.2/boxhed_kernel/src/CMakeLists.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 file(GLOB_RECURSE CPU_SOURCES *.cc *.h)
-list(REMOVE_ITEM CPU_SOURCES ${xgboost_SOURCE_DIR}/src/cli_main.cc)
+list(REMOVE_ITEM CPU_SOURCES ${boxhed_kernel_SOURCE_DIR}/src/cli_main.cc)
 
 #-- Object library
 # Object library is necessary for jvm-package, which creates its own shared library.
-add_library(objxgboost OBJECT)
-target_sources(objxgboost PRIVATE ${CPU_SOURCES})
+add_library(objboxhed_kernel OBJECT)
+target_sources(objboxhed_kernel PRIVATE ${CPU_SOURCES})
 # Skip files with factory object
 set_source_files_properties(
   predictor/predictor.cc gbm/gbm.cc tree/tree_updater.cc metric/metric.cc objective/objective.cc
   PROPERTIES SKIP_UNITY_BUILD_INCLUSION ON)
-target_sources(objxgboost PRIVATE ${RABIT_SOURCES})
+target_sources(objboxhed_kernel PRIVATE ${RABIT_SOURCES})
 
 if (USE_CUDA)
   file(GLOB_RECURSE CUDA_SOURCES *.cu *.cuh)
-  target_sources(objxgboost PRIVATE ${CUDA_SOURCES})
-  xgboost_set_cuda_flags(objxgboost)
-  target_link_libraries(objxgboost PRIVATE GPUTreeShap)
+  target_sources(objboxhed_kernel PRIVATE ${CUDA_SOURCES})
+  boxhed_kernel_set_cuda_flags(objboxhed_kernel)
+  target_link_libraries(objboxhed_kernel PRIVATE GPUTreeShap)
 endif (USE_CUDA)
 
-target_include_directories(objxgboost
+target_include_directories(objboxhed_kernel
   PRIVATE
-  ${xgboost_SOURCE_DIR}/include
-  ${xgboost_SOURCE_DIR}/dmlc-core/include
-  ${xgboost_SOURCE_DIR}/rabit/include)
-target_compile_options(objxgboost
+  ${boxhed_kernel_SOURCE_DIR}/include
+  ${boxhed_kernel_SOURCE_DIR}/dmlc-core/include
+  ${boxhed_kernel_SOURCE_DIR}/rabit/include)
+target_compile_options(objboxhed_kernel
   PRIVATE
   $<$<AND:$<CXX_COMPILER_ID:MSVC>,$<COMPILE_LANGUAGE:CXX>>:/MP>
   $<$<AND:$<NOT:$<CXX_COMPILER_ID:MSVC>>,$<COMPILE_LANGUAGE:CXX>>:-funroll-loops>)
 if (WIN32 AND MINGW)
-  target_compile_options(objxgboost PUBLIC -static-libstdc++)
+  target_compile_options(objboxhed_kernel PUBLIC -static-libstdc++)
 endif (WIN32 AND MINGW)
 
 if (MSVC)
-  target_compile_options(objxgboost PRIVATE
+  target_compile_options(objboxhed_kernel PRIVATE
     $<$<NOT:$<COMPILE_LANGUAGE:CUDA>>:/utf-8>
     -D_CRT_SECURE_NO_WARNINGS
     -D_CRT_SECURE_NO_DEPRECATE
   )
 endif (MSVC)
 
 if (ENABLE_ALL_WARNINGS)
-  target_compile_options(objxgboost PUBLIC
+  target_compile_options(objboxhed_kernel PUBLIC
     $<IF:$<COMPILE_LANGUAGE:CUDA>,-Xcompiler=-Wall -Xcompiler=-Wextra,-Wall -Wextra>)
 endif (ENABLE_ALL_WARNINGS)
 if (LOG_CAPI_INVOCATION)
-  target_compile_definitions(objxgboost PUBLIC -DLOG_CAPI_INVOCATION=1)
+  target_compile_definitions(objboxhed_kernel PUBLIC -DLOG_CAPI_INVOCATION=1)
 endif (LOG_CAPI_INVOCATION)
 
-set_target_properties(objxgboost PROPERTIES
+set_target_properties(objboxhed_kernel PROPERTIES
   POSITION_INDEPENDENT_CODE ON
   CXX_STANDARD 14
   CXX_STANDARD_REQUIRED ON)
-target_compile_definitions(objxgboost
+target_compile_definitions(objboxhed_kernel
   PRIVATE
   -DDMLC_LOG_CUSTOMIZE=1  # enable custom logging
   $<$<NOT:$<CXX_COMPILER_ID:MSVC>>:_MWAITXINTRIN_H_INCLUDED>)
 if (USE_DEBUG_OUTPUT)
-  target_compile_definitions(objxgboost PRIVATE -DXGBOOST_USE_DEBUG_OUTPUT=1)
+  target_compile_definitions(objboxhed_kernel PRIVATE -DXGBOOST_USE_DEBUG_OUTPUT=1)
 endif (USE_DEBUG_OUTPUT)
 
 if (XGBOOST_MM_PREFETCH_PRESENT)
-  target_compile_definitions(objxgboost
+  target_compile_definitions(objboxhed_kernel
     PRIVATE
     -DXGBOOST_MM_PREFETCH_PRESENT=1)
 endif(XGBOOST_MM_PREFETCH_PRESENT)
 if (XGBOOST_BUILTIN_PREFETCH_PRESENT)
-  target_compile_definitions(objxgboost
+  target_compile_definitions(objboxhed_kernel
     PRIVATE
     -DXGBOOST_BUILTIN_PREFETCH_PRESENT=1)
 endif (XGBOOST_BUILTIN_PREFETCH_PRESENT)
 
 find_package(Threads REQUIRED)
-target_link_libraries(objxgboost PUBLIC Threads::Threads ${CMAKE_THREAD_LIBS_INIT})
+target_link_libraries(objboxhed_kernel PUBLIC Threads::Threads ${CMAKE_THREAD_LIBS_INIT})
 
 if (USE_OPENMP OR USE_CUDA)  # CUDA requires OpenMP
   find_package(OpenMP REQUIRED)
-  target_link_libraries(objxgboost PUBLIC OpenMP::OpenMP_CXX)
+  target_link_libraries(objboxhed_kernel PUBLIC OpenMP::OpenMP_CXX)
 endif (USE_OPENMP OR USE_CUDA)
 
 # For MSVC: Call msvc_use_static_runtime() once again to completely
-# replace /MD with /MT. See https://github.com/dmlc/xgboost/issues/4462
+# replace /MD with /MT. See https://github.com/dmlc/boxhed_kernel/issues/4462
 # for issues caused by mixing of /MD and /MT flags
 msvc_use_static_runtime()
 
 # This grouping organises source files nicely in visual studio
 auto_source_group("${CUDA_SOURCES}")
 auto_source_group("${CPU_SOURCES}")
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/c_api/c_api.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/c_api/c_api.cc`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 #include <cstring>
 #include <fstream>
 #include <algorithm>
 #include <vector>
 #include <string>
 #include <memory>
 
-#include "xgboost/base.h"
-#include "xgboost/data.h"
-#include "xgboost/host_device_vector.h"
-#include "xgboost/learner.h"
-#include "xgboost/c_api.h"
-#include "xgboost/logging.h"
-#include "xgboost/version_config.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/learner.h"
+#include "boxhed_kernel/c_api.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/version_config.h"
+#include "boxhed_kernel/json.h"
 
 #include "c_api_error.h"
 #include "../common/io.h"
 #include "../data/adapter.h"
 #include "../data/simple_dmatrix.h"
 #include "../data/proxy_dmatrix.h"
 
-using namespace xgboost; // NOLINT(*);
+using namespace boxhed_kernel; // NOLINT(*);
 
 XGB_DLL void XGBoostVersion(int* major, int* minor, int* patch) {
   if (major) {
     *major = XGBOOST_VER_MAJOR;
   }
   if (minor) {
     *minor = XGBOOST_VER_MINOR;
@@ -58,23 +58,23 @@
   }
   *out = new std::shared_ptr<DMatrix>(DMatrix::Load(fname, silent != 0, load_row_split));
   API_END();
 }
 
 XGB_DLL int XGDMatrixCreateFromDataIter(
     void *data_handle,                  // a Java iterator
-    XGBCallbackDataIterNext *callback,  // C++ callback defined in xgboost4j.cpp
+    XGBCallbackDataIterNext *callback,  // C++ callback defined in boxhed_kernel4j.cpp
     const char *cache_info, DMatrixHandle *out) {
   API_BEGIN();
 
   std::string scache;
   if (cache_info != nullptr) {
     scache = cache_info;
   }
-  xgboost::data::IteratorAdapter<DataIterHandle, XGBCallbackDataIterNext,
+  boxhed_kernel::data::IteratorAdapter<DataIterHandle, XGBCallbackDataIterNext,
                                  XGBoostBatchCSR> adapter(data_handle, callback);
   *out = new std::shared_ptr<DMatrix> {
     DMatrix::Create(
         &adapter, std::numeric_limits<float>::quiet_NaN(),
         1, scache
     )
   };
@@ -101,51 +101,51 @@
 }
 
 #endif
 
 // Create from data iterator
 XGB_DLL int XGProxyDMatrixCreate(DMatrixHandle* out) {
   API_BEGIN();
-  *out = new std::shared_ptr<xgboost::DMatrix>(new xgboost::data::DMatrixProxy);;
+  *out = new std::shared_ptr<boxhed_kernel::DMatrix>(new boxhed_kernel::data::DMatrixProxy);;
   API_END();
 }
 
 XGB_DLL int
 XGDeviceQuantileDMatrixSetDataCudaArrayInterface(DMatrixHandle handle,
                                                  char const *c_interface_str) {
   API_BEGIN();
   CHECK_HANDLE();
-  auto p_m = static_cast<std::shared_ptr<xgboost::DMatrix> *>(handle);
+  auto p_m = static_cast<std::shared_ptr<boxhed_kernel::DMatrix> *>(handle);
   CHECK(p_m);
-  auto m =   static_cast<xgboost::data::DMatrixProxy*>(p_m->get());
+  auto m =   static_cast<boxhed_kernel::data::DMatrixProxy*>(p_m->get());
   CHECK(m) << "Current DMatrix type does not support set data.";
   m->SetData(c_interface_str);
   API_END();
 }
 
 XGB_DLL int
 XGDeviceQuantileDMatrixSetDataCudaColumnar(DMatrixHandle handle,
                                            char const *c_interface_str) {
   API_BEGIN();
   CHECK_HANDLE();
-  auto p_m = static_cast<std::shared_ptr<xgboost::DMatrix> *>(handle);
+  auto p_m = static_cast<std::shared_ptr<boxhed_kernel::DMatrix> *>(handle);
   CHECK(p_m);
-  auto m =   static_cast<xgboost::data::DMatrixProxy*>(p_m->get());
+  auto m =   static_cast<boxhed_kernel::data::DMatrixProxy*>(p_m->get());
   CHECK(m) << "Current DMatrix type does not support set data.";
   m->SetData(c_interface_str);
   API_END();
 }
 
 XGB_DLL int XGDeviceQuantileDMatrixCreateFromCallback(
     DataIterHandle iter, DMatrixHandle proxy, DataIterResetCallback *reset,
     XGDMatrixCallbackNext *next, float missing, int nthread,
     int max_bin, DMatrixHandle *out) {
   API_BEGIN();
-  *out = new std::shared_ptr<xgboost::DMatrix>{
-    xgboost::DMatrix::Create(iter, proxy, reset, next, missing, nthread, max_bin)};
+  *out = new std::shared_ptr<boxhed_kernel::DMatrix>{
+    boxhed_kernel::DMatrix::Create(iter, proxy, reset, next, missing, nthread, max_bin)};
   API_END();
 }
 // End Create from data iterator
 
 XGB_DLL int XGDMatrixCreateFromCSREx(const size_t* indptr,
                                      const unsigned* indices,
                                      const bst_float* data,
@@ -169,55 +169,55 @@
   API_BEGIN();
   data::CSCAdapter adapter(col_ptr, indices, data, nindptr - 1, num_row);
   *out = new std::shared_ptr<DMatrix>(DMatrix::Create(&adapter, std::nan(""), 1));
   API_END();
 }
 
 XGB_DLL int XGDMatrixCreateFromMat(const bst_float* data,
-                                   xgboost::bst_ulong nrow,
-                                   xgboost::bst_ulong ncol, bst_float missing,
+                                   boxhed_kernel::bst_ulong nrow,
+                                   boxhed_kernel::bst_ulong ncol, bst_float missing,
                                    DMatrixHandle* out) {
   API_BEGIN();
   data::DenseAdapter adapter(data, nrow, ncol);
   *out = new std::shared_ptr<DMatrix>(DMatrix::Create(&adapter, missing, 1));
   API_END();
 }
 
 XGB_DLL int XGDMatrixCreateFromMat_omp(const bst_float* data,  // NOLINT
-                                       xgboost::bst_ulong nrow,
-                                       xgboost::bst_ulong ncol,
+                                       boxhed_kernel::bst_ulong nrow,
+                                       boxhed_kernel::bst_ulong ncol,
                                        bst_float missing, DMatrixHandle* out,
                                        int nthread) {
   API_BEGIN();
   data::DenseAdapter adapter(data, nrow, ncol);
   *out = new std::shared_ptr<DMatrix>(DMatrix::Create(&adapter, missing, nthread));
   API_END();
 }
 
 XGB_DLL int XGDMatrixCreateFromDT(void** data, const char** feature_stypes,
-                                  xgboost::bst_ulong nrow,
-                                  xgboost::bst_ulong ncol, DMatrixHandle* out,
+                                  boxhed_kernel::bst_ulong nrow,
+                                  boxhed_kernel::bst_ulong ncol, DMatrixHandle* out,
                                   int nthread) {
   API_BEGIN();
   data::DataTableAdapter adapter(data, feature_stypes, nrow, ncol);
   *out = new std::shared_ptr<DMatrix>(
       DMatrix::Create(&adapter, std::nan(""), nthread));
   API_END();
 }
 
 XGB_DLL int XGDMatrixSliceDMatrix(DMatrixHandle handle,
                                   const int* idxset,
-                                  xgboost::bst_ulong len,
+                                  boxhed_kernel::bst_ulong len,
                                   DMatrixHandle* out) {
   return XGDMatrixSliceDMatrixEx(handle, idxset, len, out, 0);
 }
 
 XGB_DLL int XGDMatrixSliceDMatrixEx(DMatrixHandle handle,
                                     const int* idxset,
-                                    xgboost::bst_ulong len,
+                                    boxhed_kernel::bst_ulong len,
                                     DMatrixHandle* out,
                                     int allow_groups) {
   API_BEGIN();
   CHECK_HANDLE();
   if (!allow_groups) {
     CHECK_EQ(static_cast<std::shared_ptr<DMatrix>*>(handle)
                  ->get()
@@ -251,19 +251,19 @@
   }
   API_END();
 }
 
 XGB_DLL int XGDMatrixSetFloatInfo(DMatrixHandle handle,
                                   const char* field,
                                   const bst_float* info,
-                                  xgboost::bst_ulong len) {
+                                  boxhed_kernel::bst_ulong len) {
   API_BEGIN();
   CHECK_HANDLE();
   static_cast<std::shared_ptr<DMatrix>*>(handle)
-      ->get()->Info().SetInfo(field, info, xgboost::DataType::kFloat32, len);
+      ->get()->Info().SetInfo(field, info, boxhed_kernel::DataType::kFloat32, len);
   API_END();
 }
 
 XGB_DLL int XGDMatrixSetInfoFromInterface(DMatrixHandle handle,
                                           char const* field,
                                           char const* interface_c_str) {
   API_BEGIN();
@@ -272,34 +272,34 @@
       ->get()->Info().SetInfo(field, interface_c_str);
   API_END();
 }
 
 XGB_DLL int XGDMatrixSetUIntInfo(DMatrixHandle handle,
                                  const char* field,
                                  const unsigned* info,
-                                 xgboost::bst_ulong len) {
+                                 boxhed_kernel::bst_ulong len) {
   API_BEGIN();
   CHECK_HANDLE();
   static_cast<std::shared_ptr<DMatrix>*>(handle)
-      ->get()->Info().SetInfo(field, info, xgboost::DataType::kUInt32, len);
+      ->get()->Info().SetInfo(field, info, boxhed_kernel::DataType::kUInt32, len);
   API_END();
 }
 
 XGB_DLL int XGDMatrixSetStrFeatureInfo(DMatrixHandle handle, const char *field,
                                        const char **c_info,
-                                       const xgboost::bst_ulong size) {
+                                       const boxhed_kernel::bst_ulong size) {
   API_BEGIN();
   CHECK_HANDLE();
   auto &info = static_cast<std::shared_ptr<DMatrix> *>(handle)->get()->Info();
   info.SetFeatureInfo(field, c_info, size);
   API_END();
 }
 
 XGB_DLL int XGDMatrixGetStrFeatureInfo(DMatrixHandle handle, const char *field,
-                                       xgboost::bst_ulong *len,
+                                       boxhed_kernel::bst_ulong *len,
                                        const char ***out_features) {
   API_BEGIN();
   CHECK_HANDLE();
   auto m = *static_cast<std::shared_ptr<DMatrix>*>(handle);
   auto &info = static_cast<std::shared_ptr<DMatrix> *>(handle)->get()->Info();
 
   std::vector<const char *> &charp_vecs = m->GetThreadLocal().ret_vec_charp;
@@ -308,87 +308,87 @@
   info.GetFeatureInfo(field, &str_vecs);
 
   charp_vecs.resize(str_vecs.size());
   for (size_t i = 0; i < str_vecs.size(); ++i) {
     charp_vecs[i] = str_vecs[i].c_str();
   }
   *out_features = dmlc::BeginPtr(charp_vecs);
-  *len = static_cast<xgboost::bst_ulong>(charp_vecs.size());
+  *len = static_cast<boxhed_kernel::bst_ulong>(charp_vecs.size());
   API_END();
 }
 
 XGB_DLL int XGDMatrixSetDenseInfo(DMatrixHandle handle, const char *field,
-                                  void *data, xgboost::bst_ulong size,
+                                  void *data, boxhed_kernel::bst_ulong size,
                                   int type) {
   API_BEGIN();
   CHECK_HANDLE();
   auto &info = static_cast<std::shared_ptr<DMatrix> *>(handle)->get()->Info();
   CHECK(type >= 1 && type <= 4);
   info.SetInfo(field, data, static_cast<DataType>(type), size);
   API_END();
 }
 
 XGB_DLL int XGDMatrixSetGroup(DMatrixHandle handle,
                               const unsigned* group,
-                              xgboost::bst_ulong len) {
+                              boxhed_kernel::bst_ulong len) {
   API_BEGIN();
   CHECK_HANDLE();
   LOG(WARNING) << "XGDMatrixSetGroup is deprecated, use `XGDMatrixSetUIntInfo` instead.";
   static_cast<std::shared_ptr<DMatrix>*>(handle)
-      ->get()->Info().SetInfo("group", group, xgboost::DataType::kUInt32, len);
+      ->get()->Info().SetInfo("group", group, boxhed_kernel::DataType::kUInt32, len);
   API_END();
 }
 
 XGB_DLL int XGDMatrixGetFloatInfo(const DMatrixHandle handle,
                                   const char* field,
-                                  xgboost::bst_ulong* out_len,
+                                  boxhed_kernel::bst_ulong* out_len,
                                   const bst_float** out_dptr) {
   API_BEGIN();
   CHECK_HANDLE();
   const MetaInfo& info = static_cast<std::shared_ptr<DMatrix>*>(handle)->get()->Info();
   info.GetInfo(field, out_len, DataType::kFloat32, reinterpret_cast<void const**>(out_dptr));
   API_END();
 }
 
 XGB_DLL int XGDMatrixGetUIntInfo(const DMatrixHandle handle,
                                  const char *field,
-                                 xgboost::bst_ulong *out_len,
+                                 boxhed_kernel::bst_ulong *out_len,
                                  const unsigned **out_dptr) {
   API_BEGIN();
   CHECK_HANDLE();
   const MetaInfo& info = static_cast<std::shared_ptr<DMatrix>*>(handle)->get()->Info();
   info.GetInfo(field, out_len, DataType::kUInt32, reinterpret_cast<void const**>(out_dptr));
   API_END();
 }
 
 XGB_DLL int XGDMatrixNumRow(const DMatrixHandle handle,
-                            xgboost::bst_ulong *out) {
+                            boxhed_kernel::bst_ulong *out) {
   API_BEGIN();
   CHECK_HANDLE();
-  *out = static_cast<xgboost::bst_ulong>(
+  *out = static_cast<boxhed_kernel::bst_ulong>(
       static_cast<std::shared_ptr<DMatrix>*>(handle)->get()->Info().num_row_);
   API_END();
 }
 
 XGB_DLL int XGDMatrixNumCol(const DMatrixHandle handle,
-                            xgboost::bst_ulong *out) {
+                            boxhed_kernel::bst_ulong *out) {
   API_BEGIN();
   CHECK_HANDLE();
-  *out = static_cast<xgboost::bst_ulong>(
+  *out = static_cast<boxhed_kernel::bst_ulong>(
       static_cast<std::shared_ptr<DMatrix>*>(handle)->get()->Info().num_col_);
   API_END();
 }
 
-// xgboost implementation
+// boxhed_kernel implementation
 XGB_DLL int XGBoosterCreate(const DMatrixHandle dmats[],
-                            xgboost::bst_ulong len,
+                            boxhed_kernel::bst_ulong len,
                             BoosterHandle *out) {
   API_BEGIN();
   std::vector<std::shared_ptr<DMatrix> > mats;
-  for (xgboost::bst_ulong i = 0; i < len; ++i) {
+  for (boxhed_kernel::bst_ulong i = 0; i < len; ++i) {
     mats.push_back(*static_cast<std::shared_ptr<DMatrix>*>(dmats[i]));
   }
   *out = Learner::Create(mats);
   API_END();
 }
 
 XGB_DLL int XGBoosterFree(BoosterHandle handle) {
@@ -404,15 +404,15 @@
   API_BEGIN();
   CHECK_HANDLE();
   static_cast<Learner*>(handle)->SetParam(name, value);
   API_END();
 }
 
 XGB_DLL int XGBoosterGetNumFeature(BoosterHandle handle,
-                                   xgboost::bst_ulong *out) {
+                                   boxhed_kernel::bst_ulong *out) {
   API_BEGIN();
   CHECK_HANDLE();
   *out = static_cast<Learner*>(handle)->GetNumFeature();
   API_END();
 }
 
 XGB_DLL int XGBoosterLoadJsonConfig(BoosterHandle handle, char const* json_parameters) {
@@ -421,26 +421,26 @@
   std::string str {json_parameters};
   Json config { Json::Load(StringView{str.c_str(), str.size()}) };
   static_cast<Learner*>(handle)->LoadConfig(config);
   API_END();
 }
 
 XGB_DLL int XGBoosterSaveJsonConfig(BoosterHandle handle,
-                                    xgboost::bst_ulong *out_len,
+                                    boxhed_kernel::bst_ulong *out_len,
                                     char const** out_str) {
   API_BEGIN();
   CHECK_HANDLE();
   Json config { Object() };
   auto* learner = static_cast<Learner*>(handle);
   learner->Configure();
   learner->SaveConfig(&config);
   std::string& raw_str = learner->GetThreadLocal().ret_str;
   Json::Dump(config, &raw_str);
   *out_str = raw_str.c_str();
-  *out_len = static_cast<xgboost::bst_ulong>(raw_str.length());
+  *out_len = static_cast<boxhed_kernel::bst_ulong>(raw_str.length());
   API_END();
 }
 
 XGB_DLL int XGBoosterUpdateOneIter(BoosterHandle handle,
                                    int iter,
                                    DMatrixHandle dtrain) {
   API_BEGIN();
@@ -453,61 +453,61 @@
   API_END();
 }
 
 XGB_DLL int XGBoosterBoostOneIter(BoosterHandle handle,
                                   DMatrixHandle dtrain,
                                   bst_float *grad,
                                   bst_float *hess,
-                                  xgboost::bst_ulong len) {
+                                  boxhed_kernel::bst_ulong len) {
   HostDeviceVector<GradientPair> tmp_gpair;
   API_BEGIN();
   CHECK_HANDLE();
   auto* bst = static_cast<Learner*>(handle);
   auto* dtr =
       static_cast<std::shared_ptr<DMatrix>*>(dtrain);
   tmp_gpair.Resize(len);
   std::vector<GradientPair>& tmp_gpair_h = tmp_gpair.HostVector();
-  for (xgboost::bst_ulong i = 0; i < len; ++i) {
+  for (boxhed_kernel::bst_ulong i = 0; i < len; ++i) {
     tmp_gpair_h[i] = GradientPair(grad[i], hess[i]);
   }
 
   bst->BoostOneIter(0, *dtr, &tmp_gpair);
   API_END();
 }
 
 XGB_DLL int XGBoosterEvalOneIter(BoosterHandle handle,
                                  int iter,
                                  DMatrixHandle dmats[],
                                  const char* evnames[],
-                                 xgboost::bst_ulong len,
+                                 boxhed_kernel::bst_ulong len,
                                  const char** out_str) {
   API_BEGIN();
   CHECK_HANDLE();
   auto* bst = static_cast<Learner*>(handle);
   std::string& eval_str = bst->GetThreadLocal().ret_str;
 
   std::vector<std::shared_ptr<DMatrix>> data_sets;
   std::vector<std::string> data_names;
 
-  for (xgboost::bst_ulong i = 0; i < len; ++i) {
+  for (boxhed_kernel::bst_ulong i = 0; i < len; ++i) {
     data_sets.push_back(*static_cast<std::shared_ptr<DMatrix>*>(dmats[i]));
     data_names.emplace_back(evnames[i]);
   }
 
   eval_str = bst->EvalOneIter(iter, data_sets, data_names);
   *out_str = eval_str.c_str();
   API_END();
 }
 
 XGB_DLL int XGBoosterPredict(BoosterHandle handle,
                              DMatrixHandle dmat,
                              int option_mask,
                              unsigned ntree_limit,
                              int training,
-                             xgboost::bst_ulong *len,
+                             boxhed_kernel::bst_ulong *len,
                              const bst_float **out_result) {
   API_BEGIN();
   CHECK_HANDLE();
   auto *learner = static_cast<Learner*>(handle);
   auto& entry = learner->GetThreadLocal().prediction_entry;
   learner->Predict(
       *static_cast<std::shared_ptr<DMatrix>*>(dmat),
@@ -515,43 +515,43 @@
       &entry.predictions, ntree_limit,
       static_cast<bool>(training),
       (option_mask & 2) != 0,
       (option_mask & 4) != 0,
       (option_mask & 8) != 0,
       (option_mask & 16) != 0);
   *out_result = dmlc::BeginPtr(entry.predictions.ConstHostVector());
-  *len = static_cast<xgboost::bst_ulong>(entry.predictions.Size());
+  *len = static_cast<boxhed_kernel::bst_ulong>(entry.predictions.Size());
   API_END();
 }
 
 // A hidden API as cache id is not being supported yet.
 XGB_DLL int XGBoosterPredictFromDense(BoosterHandle handle, float *values,
-                                      xgboost::bst_ulong n_rows,
-                                      xgboost::bst_ulong n_cols,
+                                      boxhed_kernel::bst_ulong n_rows,
+                                      boxhed_kernel::bst_ulong n_cols,
                                       float missing,
                                       unsigned iteration_begin,
                                       unsigned iteration_end,
                                       char const* c_type,
-                                      xgboost::bst_ulong cache_id,
-                                      xgboost::bst_ulong *out_len,
+                                      boxhed_kernel::bst_ulong cache_id,
+                                      boxhed_kernel::bst_ulong *out_len,
                                       const float **out_result) {
   API_BEGIN();
   CHECK_HANDLE();
   CHECK_EQ(cache_id, 0) << "Cache ID is not supported yet";
-  auto *learner = static_cast<xgboost::Learner *>(handle);
+  auto *learner = static_cast<boxhed_kernel::Learner *>(handle);
 
-  std::shared_ptr<xgboost::data::DenseAdapter> x{
-    new xgboost::data::DenseAdapter(values, n_rows, n_cols)};
+  std::shared_ptr<boxhed_kernel::data::DenseAdapter> x{
+    new boxhed_kernel::data::DenseAdapter(values, n_rows, n_cols)};
   HostDeviceVector<float>* p_predt { nullptr };
   std::string type { c_type };
   learner->InplacePredict(x, type, missing, &p_predt, iteration_begin, iteration_end);
   CHECK(p_predt);
 
   *out_result = dmlc::BeginPtr(p_predt->HostVector());
-  *out_len = static_cast<xgboost::bst_ulong>(p_predt->Size());
+  *out_len = static_cast<boxhed_kernel::bst_ulong>(p_predt->Size());
   API_END();
 }
 
 // A hidden API as cache id is not being supported yet.
 XGB_DLL int XGBoosterPredictFromCSR(BoosterHandle handle,
                                     const size_t* indptr,
                                     const unsigned* indices,
@@ -559,57 +559,57 @@
                                     size_t nindptr,
                                     size_t nelem,
                                     size_t num_col,
                                     float missing,
                                     unsigned iteration_begin,
                                     unsigned iteration_end,
                                     char const *c_type,
-                                    xgboost::bst_ulong cache_id,
-                                    xgboost::bst_ulong *out_len,
+                                    boxhed_kernel::bst_ulong cache_id,
+                                    boxhed_kernel::bst_ulong *out_len,
                                     const float **out_result) {
   API_BEGIN();
   CHECK_HANDLE();
   CHECK_EQ(cache_id, 0) << "Cache ID is not supported yet";
-  auto *learner = static_cast<xgboost::Learner *>(handle);
+  auto *learner = static_cast<boxhed_kernel::Learner *>(handle);
 
-  std::shared_ptr<xgboost::data::CSRAdapter> x{
-    new xgboost::data::CSRAdapter(indptr, indices, data, nindptr - 1, nelem, num_col)};
+  std::shared_ptr<boxhed_kernel::data::CSRAdapter> x{
+    new boxhed_kernel::data::CSRAdapter(indptr, indices, data, nindptr - 1, nelem, num_col)};
   HostDeviceVector<float>* p_predt { nullptr };
   std::string type { c_type };
   learner->InplacePredict(x, type, missing, &p_predt, iteration_begin, iteration_end);
   CHECK(p_predt);
 
   *out_result = dmlc::BeginPtr(p_predt->HostVector());
-  *out_len = static_cast<xgboost::bst_ulong>(p_predt->Size());
+  *out_len = static_cast<boxhed_kernel::bst_ulong>(p_predt->Size());
   API_END();
 }
 
 #if !defined(XGBOOST_USE_CUDA)
 XGB_DLL int XGBoosterPredictFromArrayInterfaceColumns(BoosterHandle handle,
                                                       char const* c_json_strs,
                                                       float missing,
                                                       unsigned iteration_begin,
                                                       unsigned iteration_end,
                                                       char const* c_type,
-                                                      xgboost::bst_ulong cache_id,
-                                                      xgboost::bst_ulong *out_len,
+                                                      boxhed_kernel::bst_ulong cache_id,
+                                                      boxhed_kernel::bst_ulong *out_len,
                                                       float const** out_result) {
   API_BEGIN();
   CHECK_HANDLE();
   common::AssertGPUSupport();
   API_END();
 }
 XGB_DLL int XGBoosterPredictFromArrayInterface(BoosterHandle handle,
                                                char const* c_json_strs,
                                                float missing,
                                                unsigned iteration_begin,
                                                unsigned iteration_end,
                                                char const* c_type,
-                                               xgboost::bst_ulong cache_id,
-                                               xgboost::bst_ulong *out_len,
+                                               boxhed_kernel::bst_ulong cache_id,
+                                               boxhed_kernel::bst_ulong *out_len,
                                                const float **out_result) {
   API_BEGIN();
   CHECK_HANDLE();
   common::AssertGPUSupport();
   API_END();
 }
 #endif  // !defined(XGBOOST_USE_CUDA)
@@ -647,61 +647,61 @@
     bst->SaveModel(fo.get());
   }
   API_END();
 }
 
 XGB_DLL int XGBoosterLoadModelFromBuffer(BoosterHandle handle,
                                          const void* buf,
-                                         xgboost::bst_ulong len) {
+                                         boxhed_kernel::bst_ulong len) {
   API_BEGIN();
   CHECK_HANDLE();
   common::MemoryFixSizeBuffer fs((void*)buf, len);  // NOLINT(*)
   static_cast<Learner*>(handle)->LoadModel(&fs);
   API_END();
 }
 
 XGB_DLL int XGBoosterGetModelRaw(BoosterHandle handle,
-                                 xgboost::bst_ulong* out_len,
+                                 boxhed_kernel::bst_ulong* out_len,
                                  const char** out_dptr) {
   API_BEGIN();
   CHECK_HANDLE();
   auto *learner = static_cast<Learner*>(handle);
   std::string& raw_str = learner->GetThreadLocal().ret_str;
   raw_str.resize(0);
 
   common::MemoryBufferStream fo(&raw_str);
 
   learner->Configure();
   learner->SaveModel(&fo);
   *out_dptr = dmlc::BeginPtr(raw_str);
-  *out_len = static_cast<xgboost::bst_ulong>(raw_str.length());
+  *out_len = static_cast<boxhed_kernel::bst_ulong>(raw_str.length());
   API_END();
 }
 
 // The following two functions are `Load` and `Save` for memory based
 // serialization methods. E.g. Python pickle.
 XGB_DLL int XGBoosterSerializeToBuffer(BoosterHandle handle,
-                                       xgboost::bst_ulong *out_len,
+                                       boxhed_kernel::bst_ulong *out_len,
                                        const char **out_dptr) {
   API_BEGIN();
   CHECK_HANDLE();
   auto *learner = static_cast<Learner*>(handle);
   std::string &raw_str = learner->GetThreadLocal().ret_str;
   raw_str.resize(0);
   common::MemoryBufferStream fo(&raw_str);
   learner->Configure();
   learner->Save(&fo);
   *out_dptr = dmlc::BeginPtr(raw_str);
-  *out_len = static_cast<xgboost::bst_ulong>(raw_str.length());
+  *out_len = static_cast<boxhed_kernel::bst_ulong>(raw_str.length());
   API_END();
 }
 
 XGB_DLL int XGBoosterUnserializeFromBuffer(BoosterHandle handle,
                                            const void *buf,
-                                           xgboost::bst_ulong len) {
+                                           boxhed_kernel::bst_ulong len) {
   API_BEGIN();
   CHECK_HANDLE();
   common::MemoryFixSizeBuffer fs((void*)buf, len);  // NOLINT(*)
   static_cast<Learner*>(handle)->Load(&fs);
   API_END();
 }
 
@@ -744,44 +744,44 @@
   CHECK(p_out);
   *out = p_out;
   API_END();
 }
 
 inline void XGBoostDumpModelImpl(BoosterHandle handle, const FeatureMap &fmap,
                                  int with_stats, const char *format,
-                                 xgboost::bst_ulong *len,
+                                 boxhed_kernel::bst_ulong *len,
                                  const char ***out_models) {
   auto *bst = static_cast<Learner*>(handle);
   std::vector<std::string>& str_vecs = bst->GetThreadLocal().ret_vec_str;
   std::vector<const char*>& charp_vecs = bst->GetThreadLocal().ret_vec_charp;
   str_vecs = bst->DumpModel(fmap, with_stats != 0, format);
   charp_vecs.resize(str_vecs.size());
   for (size_t i = 0; i < str_vecs.size(); ++i) {
     charp_vecs[i] = str_vecs[i].c_str();
   }
   *out_models = dmlc::BeginPtr(charp_vecs);
-  *len = static_cast<xgboost::bst_ulong>(charp_vecs.size());
+  *len = static_cast<boxhed_kernel::bst_ulong>(charp_vecs.size());
 }
 
 XGB_DLL int XGBoosterDumpModel(BoosterHandle handle,
                                const char* fmap,
                                int with_stats,
-                               xgboost::bst_ulong* len,
+                               boxhed_kernel::bst_ulong* len,
                                const char*** out_models) {
   API_BEGIN();
   CHECK_HANDLE();
   return XGBoosterDumpModelEx(handle, fmap, with_stats, "text", len, out_models);
   API_END();
 }
 
 XGB_DLL int XGBoosterDumpModelEx(BoosterHandle handle,
                                  const char* fmap,
                                  int with_stats,
                                  const char *format,
-                                 xgboost::bst_ulong* len,
+                                 boxhed_kernel::bst_ulong* len,
                                  const char*** out_models) {
   API_BEGIN();
   CHECK_HANDLE();
   FeatureMap featmap;
   if (strlen(fmap) != 0) {
     std::unique_ptr<dmlc::Stream> fs(
         dmlc::Stream::Create(fmap, "r"));
@@ -793,27 +793,27 @@
 }
 
 XGB_DLL int XGBoosterDumpModelWithFeatures(BoosterHandle handle,
                                            int fnum,
                                            const char** fname,
                                            const char** ftype,
                                            int with_stats,
-                                           xgboost::bst_ulong* len,
+                                           boxhed_kernel::bst_ulong* len,
                                            const char*** out_models) {
   return XGBoosterDumpModelExWithFeatures(handle, fnum, fname, ftype, with_stats,
                                           "text", len, out_models);
 }
 
 XGB_DLL int XGBoosterDumpModelExWithFeatures(BoosterHandle handle,
                                              int fnum,
                                              const char** fname,
                                              const char** ftype,
                                              int with_stats,
                                              const char *format,
-                                             xgboost::bst_ulong* len,
+                                             boxhed_kernel::bst_ulong* len,
                                              const char*** out_models) {
   API_BEGIN();
   CHECK_HANDLE();
   FeatureMap featmap;
   for (int i = 0; i < fnum; ++i) {
     featmap.PushBack(i, fname[i], ftype[i]);
   }
@@ -850,27 +850,27 @@
   } else {
     bst->SetAttr(key, value);
   }
   API_END();
 }
 
 XGB_DLL int XGBoosterGetAttrNames(BoosterHandle handle,
-                                  xgboost::bst_ulong* out_len,
+                                  boxhed_kernel::bst_ulong* out_len,
                                   const char*** out) {
   API_BEGIN();
   CHECK_HANDLE();
   auto *learner = static_cast<Learner *>(handle);
   std::vector<std::string> &str_vecs = learner->GetThreadLocal().ret_vec_str;
   std::vector<const char *> &charp_vecs =
       learner->GetThreadLocal().ret_vec_charp;
   str_vecs = learner->GetAttrNames();
   charp_vecs.resize(str_vecs.size());
   for (size_t i = 0; i < str_vecs.size(); ++i) {
     charp_vecs[i] = str_vecs[i].c_str();
   }
   *out = dmlc::BeginPtr(charp_vecs);
-  *out_len = static_cast<xgboost::bst_ulong>(charp_vecs.size());
+  *out_len = static_cast<boxhed_kernel::bst_ulong>(charp_vecs.size());
   API_END();
 }
 
 // force link rabit
 static DMLC_ATTRIBUTE_UNUSED int XGBOOST_LINK_RABIT_C_API_ = RabitLinkTag();
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/c_api/c_api.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/c_api/c_api.cu`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright (c) 2019-2020 by Contributors
-#include "xgboost/data.h"
-#include "xgboost/c_api.h"
-#include "xgboost/learner.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/c_api.h"
+#include "boxhed_kernel/learner.h"
 #include "c_api_error.h"
 #include "../data/device_adapter.cuh"
 
-using namespace xgboost;  // NOLINT
+using namespace boxhed_kernel;  // NOLINT
 
 XGB_DLL int XGDMatrixCreateFromArrayInterfaceColumns(char const* c_json_strs,
                                                      bst_float missing,
                                                      int nthread,
                                                      DMatrixHandle* out) {
   API_BEGIN();
   std::string json_str{c_json_strs};
@@ -33,16 +33,16 @@
 // A hidden API as cache id is not being supported yet.
 XGB_DLL int XGBoosterPredictFromArrayInterfaceColumns(BoosterHandle handle,
                                                       char const* c_json_strs,
                                                       float missing,
                                                       unsigned iteration_begin,
                                                       unsigned iteration_end,
                                                       char const* c_type,
-                                                      xgboost::bst_ulong cache_id,
-                                                      xgboost::bst_ulong *out_len,
+                                                      boxhed_kernel::bst_ulong cache_id,
+                                                      boxhed_kernel::bst_ulong *out_len,
                                                       float const** out_result) {
   API_BEGIN();
   CHECK_HANDLE();
   CHECK_EQ(cache_id, 0) << "Cache ID is not supported yet";
   auto *learner = static_cast<Learner*>(handle);
 
   std::string json_str{c_json_strs};
@@ -50,27 +50,27 @@
   HostDeviceVector<float>* p_predt { nullptr };
   std::string type { c_type };
   learner->InplacePredict(x, type, missing, &p_predt, iteration_begin, iteration_end);
   CHECK(p_predt);
   CHECK(p_predt->DeviceCanRead());
 
   *out_result = p_predt->ConstDevicePointer();
-  *out_len = static_cast<xgboost::bst_ulong>(p_predt->Size());
+  *out_len = static_cast<boxhed_kernel::bst_ulong>(p_predt->Size());
 
   API_END();
 }
 // A hidden API as cache id is not being supported yet.
 XGB_DLL int XGBoosterPredictFromArrayInterface(BoosterHandle handle,
                                                char const* c_json_strs,
                                                float missing,
                                                unsigned iteration_begin,
                                                unsigned iteration_end,
                                                char const* c_type,
-                                               xgboost::bst_ulong cache_id,
-                                               xgboost::bst_ulong *out_len,
+                                               boxhed_kernel::bst_ulong cache_id,
+                                               boxhed_kernel::bst_ulong *out_len,
                                                float const** out_result) {
   API_BEGIN();
   CHECK_HANDLE();
   CHECK_EQ(cache_id, 0) << "Cache ID is not supported yet";
   auto *learner = static_cast<Learner*>(handle);
 
   std::string json_str{c_json_strs};
@@ -78,11 +78,11 @@
   HostDeviceVector<float>* p_predt { nullptr };
   std::string type { c_type };
   learner->InplacePredict(x, type, missing, &p_predt, iteration_begin, iteration_end);
   CHECK(p_predt);
   CHECK(p_predt->DeviceCanRead());
 
   *out_result = p_predt->ConstDevicePointer();
-  *out_len = static_cast<xgboost::bst_ulong>(p_predt->Size());
+  *out_len = static_cast<boxhed_kernel::bst_ulong>(p_predt->Size());
 
   API_END();
 }
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/c_api/c_api_error.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/c_api/c_api_error.h`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/cli_main.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/cli_main.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 /*!
  * Copyright 2014-2020 by Contributors
  * \file cli_main.cc
- * \brief The command line interface program of xgboost.
+ * \brief The command line interface program of boxhed_kernel.
  *  This file is not included in dynamic library.
  */
 #define _CRT_SECURE_NO_WARNINGS
 #define _CRT_SECURE_NO_DEPRECATE
 #define NOMINMAX
 #include <dmlc/timer.h>
 
-#include <xgboost/learner.h>
-#include <xgboost/data.h>
-#include <xgboost/json.h>
-#include <xgboost/logging.h>
-#include <xgboost/parameter.h>
+#include <boxhed_kernel/learner.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/json.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/parameter.h>
 
 #include <iomanip>
 #include <ctime>
 #include <string>
 #include <cstdio>
 #include <cstring>
 #include <vector>
 #include "common/common.h"
 #include "common/config.h"
 #include "common/io.h"
 #include "common/version.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 enum CLITask {
   kTrain = 0,
   kDumpModel = 1,
   kPredict = 2
 };
 
 struct CLIParam : public XGBoostParameter<CLIParam> {
@@ -152,19 +152,19 @@
 };
 
 constexpr char const* const CLIParam::kNull;
 
 DMLC_REGISTER_PARAMETER(CLIParam);
 
 std::string CliHelp() {
-  return "Use xgboost -h for showing help information.\n";
+  return "Use boxhed_kernel -h for showing help information.\n";
 }
 
 void CLIError(dmlc::Error const& e) {
-  std::cerr << "Error running xgboost:\n\n"
+  std::cerr << "Error running boxhed_kernel:\n\n"
             << e.what() << "\n"
             << CliHelp()
             << std::endl;
 }
 
 class CLI {
   CLIParam param_;
@@ -372,15 +372,15 @@
       fo->Write(str.c_str(), str.size());
     } else {
       learner->SaveModel(fo.get());
     }
   }
 
   void PrintHelp() const {
-    std::cout << "Usage: xgboost [ -h ] [ -V ] [ config file ] [ arguments ]" << std::endl;
+    std::cout << "Usage: boxhed_kernel [ -h ] [ -V ] [ config file ] [ arguments ]" << std::endl;
     std::stringstream ss;
     ss << R"(
   Options and arguments:
 
     -h, --help
        Print this message.
 
@@ -391,15 +391,15 @@
        Extra parameters that are not specified in config file, see below.
 
   Config file specifies the configuration for both training and testing.  Each line
   containing the [attribute] = [value] configuration.
 
   General XGBoost parameters:
 
-    https://xgboost.readthedocs.io/en/latest/parameter.html
+    https://boxhed_kernel.readthedocs.io/en/latest/parameter.html
 
   Command line interface specfic parameters:
 
 )";
 
     std::string help = param_.__DOC__();
     auto splited = common::Split(help, '\n');
@@ -497,30 +497,30 @@
         CLIDumpModel();
         break;
       case kPredict:
         CLIPredict();
         break;
       }
     } catch (dmlc::Error const& e) {
-      xgboost::CLIError(e);
+      boxhed_kernel::CLIError(e);
       return 1;
     }
     return 0;
   }
 
   ~CLI() {
     rabit::Finalize();
   }
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 int main(int argc, char *argv[]) {
   try {
-    xgboost::CLI cli(argc, argv);
+    boxhed_kernel::CLI cli(argc, argv);
     return cli.Run();
   } catch (dmlc::Error const& e) {
     // This captures only the initialization error.
-    xgboost::CLIError(e);
+    boxhed_kernel::CLIError(e);
     return 1;
   }
   return 0;
 }
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/base64.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/base64.h`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
  * \brief data stream support to input and output from/to base64 stream
  * base64 is easier to store and pass as text format in mapreduce
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_COMMON_BASE64_H_
 #define XGBOOST_COMMON_BASE64_H_
 
-#include <xgboost/logging.h>
+#include <boxhed_kernel/logging.h>
 #include <cctype>
 #include <cstdio>
 #include <string>
 #include "./io.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 /*! \brief buffer reader of the stream that allows you to get */
 class StreamBufferReader {
  public:
   explicit StreamBufferReader(size_t buffer_size)
       :stream_(NULL),
        read_len_(1), read_ptr_(1) {
@@ -264,9 +264,9 @@
     if (out_buf.length() != 0) {
       fp->Write(&out_buf[0], out_buf.length());
       out_buf.clear();
     }
   }
 };
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_BASE64_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/bitfield.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/bitfield.h`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 #if defined(__CUDACC__)
 #include <thrust/copy.h>
 #include <thrust/device_ptr.h>
 #include "device_helpers.cuh"
 #endif  // defined(__CUDACC__)
 
-#include "xgboost/span.h"
+#include "boxhed_kernel/span.h"
 #include "common.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 #if defined(__CUDACC__)
 using BitFieldAtomicType = unsigned long long;  // NOLINT
 
 __forceinline__ __device__ BitFieldAtomicType AtomicOr(BitFieldAtomicType* address,
                                                        BitFieldAtomicType val) {
   BitFieldAtomicType old = *address, assumed;  // NOLINT
@@ -222,10 +222,10 @@
 // Format: <Const><Direction>BitField<size of underlying type in bits>, underlying type
 // must be unsigned.
 using LBitField64 = BitFieldContainer<uint64_t, LBitsPolicy<uint64_t>>;
 using RBitField8 = BitFieldContainer<uint8_t, RBitsPolicy<unsigned char>>;
 
 using LBitField32 = BitFieldContainer<uint32_t, LBitsPolicy<uint32_t>>;
 using CLBitField32 = BitFieldContainer<uint32_t, LBitsPolicy<uint32_t, true>, true>;
-}       // namespace xgboost
+}       // namespace boxhed_kernel
 
 #endif  // XGBOOST_COMMON_BITFIELD_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/categorical.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/categorical.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /*!
  * Copyright 2020 by XGBoost Contributors
  * \file categorical.h
  */
 #ifndef XGBOOST_COMMON_CATEGORICAL_H_
 #define XGBOOST_COMMON_CATEGORICAL_H_
 
-#include "xgboost/base.h"
-#include "xgboost/data.h"
-#include "xgboost/span.h"
-#include "xgboost/parameter.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/span.h"
+#include "boxhed_kernel/parameter.h"
 #include "bitfield.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 // Cast the categorical type.
 template <typename T>
 XGBOOST_DEVICE bst_cat_t AsCat(T const& v) {
   return static_cast<bst_cat_t>(v);
 }
 
@@ -41,10 +41,10 @@
   CLBitField32 const s_cats(cats);
   return !s_cats.Check(cat);
 }
 
 using CatBitField = LBitField32;
 using KCatBitField = CLBitField32;
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_COMMON_CATEGORICAL_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/charconv.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/charconv.cc`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  */
 #include <algorithm>
 #include <cassert>
 #include <cinttypes>
 #include <cstring>
 #include <cmath>
 
-#include "xgboost/logging.h"
+#include "boxhed_kernel/logging.h"
 #include "charconv.h"
 
 #if defined(_MSC_VER)
 #include <intrin.h>
 #endif
 
 /*
@@ -50,15 +50,15 @@
  * {low, value, high}
  *
  * 3 values, representing round down, no rounding, and round up.  In the original
  * implementation and paper, variables representing these 3 values are typically postfixed
  * with m, r, p like {vr, vm, vp}.  Here we name them more verbosely.
  */
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace detail {
 static constexpr char kItoaLut[200] = {
     '0', '0', '0', '1', '0', '2', '0', '3', '0', '4', '0', '5', '0', '6', '0',
     '7', '0', '8', '0', '9', '1', '0', '1', '1', '1', '2', '1', '3', '1', '4',
     '1', '5', '1', '6', '1', '7', '1', '8', '1', '9', '2', '0', '2', '1', '2',
     '2', '2', '3', '2', '4', '2', '5', '2', '6', '2', '7', '2', '8', '2', '9',
     '3', '0', '3', '1', '3', '2', '3', '3', '3', '4', '3', '5', '3', '6', '3',
@@ -935,8 +935,8 @@
     // overflow here.
     f_e2++;
   }
   *result = IEEE754::Encode({f_m2, f_e2}, signed_mantissa);
   return {};
 }
 }  // namespace detail
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/charconv.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/charconv.h`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 #define XGBOOST_COMMON_CHARCONV_H_
 
 #include <cstddef>
 #include <system_error>
 #include <iterator>
 #include <limits>
 
-#include "xgboost/logging.h"
+#include "boxhed_kernel/logging.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 struct to_chars_result {  // NOLINT
   char* ptr;
   std::errc ec;
 };
 
 struct from_chars_result {  // NOLINT
@@ -94,10 +94,10 @@
 
 inline from_chars_result from_chars(const char *buffer, const char *end, // NOLINT
                                     float &value) {  // NOLINT
   from_chars_result res =
       detail::FromCharFloatImpl(buffer, std::distance(buffer, end), &value);
   return res;
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif   // XGBOOST_COMMON_CHARCONV_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/column_matrix.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/column_matrix.h`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #define XGBOOST_COMMON_COLUMN_MATRIX_H_
 
 #include <limits>
 #include <vector>
 #include <memory>
 #include "hist_util.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 class ColumnMatrix;
 /*! \brief column type */
 enum ColumnType {
   kDenseColumn,
   kSparseColumn
@@ -240,15 +240,15 @@
             local_index[idx + rid] = index[i];
         }
       }
     } else {
       /* to handle rows in all batches, sum of all batch sizes equal to gmat.row_ptr.size() - 1 */
       size_t rbegin = 0;
       for (const auto &batch : gmat.p_fmat->GetBatches<SparsePage>()) {
-        const xgboost::Entry* data_ptr = batch.data.HostVector().data();
+        const boxhed_kernel::Entry* data_ptr = batch.data.HostVector().data();
         const std::vector<bst_row_t>& offset_vec = batch.offset.HostVector();
         const size_t batch_size = batch.Size();
         CHECK_LT(batch_size, offset_vec.size());
         for (size_t rid = 0; rid < batch_size; ++rid) {
           const size_t size = offset_vec[rid + 1] - offset_vec[rid];
           SparsePage::Inst inst = {data_ptr + offset_vec[rid], size};
           const size_t ibegin = gmat.row_ptr[rbegin + rid];
@@ -275,15 +275,15 @@
     std::vector<size_t> num_nonzeros;
     num_nonzeros.resize(nfeature);
     std::fill(num_nonzeros.begin(), num_nonzeros.end(), 0);
 
     T* local_index = reinterpret_cast<T*>(&index_[0]);
     size_t rbegin = 0;
     for (const auto &batch : gmat.p_fmat->GetBatches<SparsePage>()) {
-      const xgboost::Entry* data_ptr = batch.data.HostVector().data();
+      const boxhed_kernel::Entry* data_ptr = batch.data.HostVector().data();
       const std::vector<bst_row_t>& offset_vec = batch.offset.HostVector();
       const size_t batch_size = batch.Size();
       CHECK_LT(batch_size, offset_vec.size());
       for (size_t rid = 0; rid < batch_size; ++rid) {
         const size_t ibegin = gmat.row_ptr[rbegin + rid];
         const size_t iend = gmat.row_ptr[rbegin + rid + 1];
         size_t fid = 0;
@@ -339,9 +339,9 @@
   uint32_t* index_base_;
   std::vector<bool> missing_flags_;
   BinTypeSize bins_type_size_;
   bool any_missing_;
 };
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_COLUMN_MATRIX_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/common.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/common.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /*!
  * Copyright 2015-2019 by Contributors
  * \file common.cc
  * \brief Enable all kinds of global variables in common.
  */
 #include <dmlc/thread_local.h>
-#include <xgboost/logging.h>
+#include <boxhed_kernel/logging.h>
 
 #include "common.h"
 #include "./random.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 /*! \brief thread local entry for random. */
 struct RandomThreadLocalEntry {
   /*! \brief the random engine instance. */
   GlobalRandomEngine engine;
 };
 
@@ -26,8 +26,8 @@
 #if !defined(XGBOOST_USE_CUDA)
 int AllVisibleGPUs() {
   return 0;
 }
 #endif  // !defined(XGBOOST_USE_CUDA)
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/common.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/common.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
  * Copyright 2015-2018 by Contributors
  * \file common.h
  * \brief Common utilities
  */
 #ifndef XGBOOST_COMMON_COMMON_H_
 #define XGBOOST_COMMON_COMMON_H_
 
-#include <xgboost/base.h>
-#include <xgboost/logging.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/logging.h>
 
 #include <algorithm>
 #include <exception>
 #include <functional>
 #include <limits>
 #include <type_traits>
 #include <vector>
@@ -46,15 +46,15 @@
                                        std::to_string(line)).what();
   }
   return code;
 }
 #endif  // defined(__CUDACC__)
 }  // namespace dh
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 /*!
  * \brief Split a string by delimiter
  * \param s String to be splitted.
  * \param delim The delimiter.
  */
 inline std::vector<std::string> Split(const std::string& s, char delim) {
@@ -169,9 +169,9 @@
   std::iota(result.begin(), result.end(), 0);
   std::stable_sort(
       result.begin(), result.end(),
       [&array, comp](Idx const &l, Idx const &r) { return comp(array[l], array[r]); });
   return result;
 }
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_COMMON_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/compressed_iterator.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/compressed_iterator.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /*!
  * Copyright 2017 by Contributors
  * \file compressed_iterator.h
  */
 #pragma once
-#include <xgboost/base.h>
+#include <boxhed_kernel/base.h>
 #include <cmath>
 #include <cstddef>
 #include <algorithm>
 
 #include "common.h"
 
 #ifdef __CUDACC__
 #include "device_helpers.cuh"
 #endif  // __CUDACC__
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 using CompressedByteT = unsigned char;
 
 namespace detail {
 inline void SetBit(CompressedByteT *byte, int bit_idx) {
   *byte |= 1 << bit_idx;
@@ -216,8 +216,8 @@
   XGBOOST_DEVICE reference operator[](size_t idx) const {
     self_type offset = (*this);
     offset.offset_ += idx;
     return *offset;
   }
 };
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/config.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/config.h`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 #include <istream>
 #include <sstream>
 #include <vector>
 #include <regex>
 #include <iterator>
 #include <utility>
 
-#include "xgboost/logging.h"
+#include "boxhed_kernel/logging.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 /*!
  * \brief Implementation of config reader
  */
 class ConfigParser {
  public:
   /*!
@@ -166,9 +166,9 @@
       LOG(FATAL) << "This line is not a valid key-value pair: " << str;
     }
     return true;
   }
 };
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_CONFIG_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/device_helpers.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/device_helpers.cu`

 * *Files 18% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 namespace dh {
 
 #if __CUDACC_VER_MAJOR__ > 9
 constexpr std::size_t kUuidLength =
     sizeof(std::declval<cudaDeviceProp>().uuid) / sizeof(uint64_t);
 
 void GetCudaUUID(int world_size, int rank, int device_ord,
-                 xgboost::common::Span<uint64_t, kUuidLength> uuid) {
+                 boxhed_kernel::common::Span<uint64_t, kUuidLength> uuid) {
   cudaDeviceProp prob;
   safe_cuda(cudaGetDeviceProperties(&prob, device_ord));
   std::memcpy(uuid.data(), static_cast<void*>(&(prob.uuid)), sizeof(prob.uuid));
 }
 
-std::string PrintUUID(xgboost::common::Span<uint64_t, kUuidLength> uuid) {
+std::string PrintUUID(boxhed_kernel::common::Span<uint64_t, kUuidLength> uuid) {
   std::stringstream ss;
   for (auto v : uuid) {
     ss << std::hex << v;
   }
   return ss.str();
 }
 
@@ -40,26 +40,26 @@
   device_ordinal_ = _device_ordinal;
   int32_t const rank = rabit::GetRank();
 
 #if __CUDACC_VER_MAJOR__ > 9
   int32_t const world = rabit::GetWorldSize();
 
   std::vector<uint64_t> uuids(world * kUuidLength, 0);
-  auto s_uuid = xgboost::common::Span<uint64_t>{uuids.data(), uuids.size()};
+  auto s_uuid = boxhed_kernel::common::Span<uint64_t>{uuids.data(), uuids.size()};
   auto s_this_uuid = s_uuid.subspan(rank * kUuidLength, kUuidLength);
   GetCudaUUID(world, rank, device_ordinal_, s_this_uuid);
 
   // No allgather yet.
   rabit::Allreduce<rabit::op::Sum, uint64_t>(uuids.data(), uuids.size());
 
-  std::vector<xgboost::common::Span<uint64_t, kUuidLength>> converted(world);;
+  std::vector<boxhed_kernel::common::Span<uint64_t, kUuidLength>> converted(world);;
   size_t j = 0;
   for (size_t i = 0; i < uuids.size(); i += kUuidLength) {
     converted[j] =
-        xgboost::common::Span<uint64_t, kUuidLength>{uuids.data() + i, kUuidLength};
+        boxhed_kernel::common::Span<uint64_t, kUuidLength>{uuids.data() + i, kUuidLength};
     j++;
   }
 
   auto iter = std::unique(converted.begin(), converted.end());
   auto n_uniques = std::distance(converted.begin(), iter);
   CHECK_EQ(n_uniques, world)
       << "Multiple processes within communication group running on same CUDA "
@@ -107,15 +107,15 @@
 
 AllReducer::~AllReducer() {
 #ifdef XGBOOST_USE_NCCL
   if (initialised_) {
     dh::safe_cuda(cudaStreamDestroy(stream_));
     ncclCommDestroy(comm_);
   }
-  if (xgboost::ConsoleLogger::ShouldLog(xgboost::ConsoleLogger::LV::kDebug)) {
+  if (boxhed_kernel::ConsoleLogger::ShouldLog(boxhed_kernel::ConsoleLogger::LV::kDebug)) {
     LOG(CONSOLE) << "======== NCCL Statistics========";
     LOG(CONSOLE) << "AllReduce calls: " << allreduce_calls_;
     LOG(CONSOLE) << "AllReduce total MiB communicated: " << allreduce_bytes_/1048576;
   }
 #endif  // XGBOOST_USE_NCCL
 }
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/device_helpers.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/device_helpers.cuh`

 * *Files 8% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 #include <chrono>
 #include <numeric>
 #include <sstream>
 #include <string>
 #include <vector>
 #include <tuple>
 
-#include "xgboost/logging.h"
-#include "xgboost/host_device_vector.h"
-#include "xgboost/span.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/span.h"
 
 #include "common.h"
 
 #ifdef XGBOOST_USE_NCCL
 #include "nccl.h"
 #endif  // XGBOOST_USE_NCCL
 
@@ -173,15 +173,15 @@
   dh::safe_cuda(cudaDeviceGetAttribute
                 (&max_shared_memory, cudaDevAttrMaxSharedMemoryPerBlockOptin,
                  device_idx));
   return size_t(max_shared_memory);
 }
 
 inline void CheckComputeCapability() {
-  for (int d_idx = 0; d_idx < xgboost::common::AllVisibleGPUs(); ++d_idx) {
+  for (int d_idx = 0; d_idx < boxhed_kernel::common::AllVisibleGPUs(); ++d_idx) {
     cudaDeviceProp prop;
     safe_cuda(cudaGetDeviceProperties(&prop, d_idx));
     std::ostringstream oss;
     oss << "CUDA Capability Major/Minor version number: " << prop.major << "."
         << prop.minor << " is insufficient.  Need >=3.5";
     int failed = prop.major < 3 || (prop.major == 3 && prop.minor < 5);
     if (failed) LOG(WARNING) << oss.str() << " for device: " << d_idx;
@@ -192,25 +192,25 @@
                                      size_t ibyte, unsigned char b) {
   atomicOr(&buffer[ibyte / sizeof(unsigned int)],
            static_cast<unsigned int>(b)
                << (ibyte % (sizeof(unsigned int)) * 8));
 }
 
 template <typename T>
-__device__ xgboost::common::Range GridStrideRange(T begin, T end) {
+__device__ boxhed_kernel::common::Range GridStrideRange(T begin, T end) {
   begin += blockDim.x * blockIdx.x + threadIdx.x;
-  xgboost::common::Range r(begin, end);
+  boxhed_kernel::common::Range r(begin, end);
   r.Step(gridDim.x * blockDim.x);
   return r;
 }
 
 template <typename T>
-__device__ xgboost::common::Range BlockStrideRange(T begin, T end) {
+__device__ boxhed_kernel::common::Range BlockStrideRange(T begin, T end) {
   begin += threadIdx.x;
-  xgboost::common::Range r(begin, end);
+  boxhed_kernel::common::Range r(begin, end);
   r.Step(blockDim.x);
   return r;
 }
 
 // Threadblock iterates over range, filling with value. Requires all threads in
 // block to be active.
 template <typename IterT, typename ValueT>
@@ -271,15 +271,15 @@
 
 template <int ITEMS_PER_THREAD = 8, int BLOCK_THREADS = 256, typename L>
 inline void LaunchN(int device_idx, size_t n, cudaStream_t stream, L lambda) {
   if (n == 0) {
     return;
   }
   const int GRID_SIZE =
-      static_cast<int>(xgboost::common::DivRoundUp(n, ITEMS_PER_THREAD * BLOCK_THREADS));
+      static_cast<int>(boxhed_kernel::common::DivRoundUp(n, ITEMS_PER_THREAD * BLOCK_THREADS));
   LaunchNKernel<<<GRID_SIZE, BLOCK_THREADS, 0, stream>>>(  // NOLINT
       static_cast<size_t>(0), n, lambda);
 }
 
 // Default stream version
 template <int ITEMS_PER_THREAD = 8, int BLOCK_THREADS = 256, typename L>
 inline void LaunchN(int device_idx, size_t n, L lambda) {
@@ -317,24 +317,24 @@
     }
   };
   DeviceStats stats_;
   std::mutex mutex_;
 
 public:
   void RegisterAllocation(void *ptr, size_t n) {
-    if (!xgboost::ConsoleLogger::ShouldLog(xgboost::ConsoleLogger::LV::kDebug)) {
+    if (!boxhed_kernel::ConsoleLogger::ShouldLog(boxhed_kernel::ConsoleLogger::LV::kDebug)) {
       return;
     }
     std::lock_guard<std::mutex> guard(mutex_);
     int current_device;
     safe_cuda(cudaGetDevice(&current_device));
     stats_.RegisterAllocation(ptr, n);
   }
   void RegisterDeallocation(void *ptr, size_t n) {
-    if (!xgboost::ConsoleLogger::ShouldLog(xgboost::ConsoleLogger::LV::kDebug)) {
+    if (!boxhed_kernel::ConsoleLogger::ShouldLog(boxhed_kernel::ConsoleLogger::LV::kDebug)) {
       return;
     }
     std::lock_guard<std::mutex> guard(mutex_);
     int current_device;
     safe_cuda(cudaGetDevice(&current_device));
     stats_.RegisterDeallocation(ptr, n, current_device);
   }
@@ -346,15 +346,15 @@
   }
   void Clear()
   {
     stats_ = DeviceStats();
   }
 
   void Log() {
-    if (!xgboost::ConsoleLogger::ShouldLog(xgboost::ConsoleLogger::LV::kDebug)) {
+    if (!boxhed_kernel::ConsoleLogger::ShouldLog(boxhed_kernel::ConsoleLogger::LV::kDebug)) {
       return;
     }
     std::lock_guard<std::mutex> guard(mutex_);
     int current_device;
     safe_cuda(cudaGetDevice(&current_device));
     LOG(CONSOLE) << "======== Device " << current_device << " Memory Allocations: "
       << " ========";
@@ -467,15 +467,15 @@
     GlobalMemoryLogger().RegisterDeallocation(ptr.get(), n * sizeof(T));
     GetGlobalCachingAllocator().DeviceFree(ptr.get());
   }
   XGBOOST_DEVICE void construct(T *) {}  // NOLINT
 };
 }  // namespace detail
 
-// Declare xgboost allocators
+// Declare boxhed_kernel allocators
 // Replacement of allocator with custom backend should occur here
 template <typename T>
 using XGBDeviceAllocator = detail::XGBDefaultDeviceAllocatorImpl<T>;
 /*! Be careful that the initialization constructor is a no-op, which means calling
  *  `vec.resize(n)` won't initialize the memory region to 0. Instead use
  * `vec.resize(n, 0)`*/
 template <typename T>
@@ -518,29 +518,29 @@
  * \brief Copies device span to std::vector.
  *
  * \tparam  T Generic type parameter.
  * \param [in,out]  dst Copy destination.
  * \param           src Copy source. Must be device memory.
  */
 template <typename T>
-void CopyDeviceSpanToVector(std::vector<T> *dst, xgboost::common::Span<T> src) {
+void CopyDeviceSpanToVector(std::vector<T> *dst, boxhed_kernel::common::Span<T> src) {
   CHECK_EQ(dst->size(), src.size());
   dh::safe_cuda(cudaMemcpyAsync(dst->data(), src.data(), dst->size() * sizeof(T),
                                 cudaMemcpyDeviceToHost));
 }
 
 /**
  * \brief Copies const device span to std::vector.
  *
  * \tparam  T Generic type parameter.
  * \param [in,out]  dst Copy destination.
  * \param           src Copy source. Must be device memory.
  */
 template <typename T>
-void CopyDeviceSpanToVector(std::vector<T> *dst, xgboost::common::Span<const T> src) {
+void CopyDeviceSpanToVector(std::vector<T> *dst, boxhed_kernel::common::Span<const T> src) {
   CHECK_EQ(dst->size(), src.size());
   dh::safe_cuda(cudaMemcpyAsync(dst->data(), src.data(), dst->size() * sizeof(T),
                                 cudaMemcpyDeviceToHost));
 }
 
 template <class HContainer, class DContainer>
 void CopyToD(HContainer const &h, DContainer *d) {
@@ -561,26 +561,26 @@
 struct PinnedMemory {
   void *temp_storage{nullptr};
   size_t temp_storage_bytes{0};
 
   ~PinnedMemory() { Free(); }
 
   template <typename T>
-  xgboost::common::Span<T> GetSpan(size_t size) {
+  boxhed_kernel::common::Span<T> GetSpan(size_t size) {
     size_t num_bytes = size * sizeof(T);
     if (num_bytes > temp_storage_bytes) {
       Free();
       safe_cuda(cudaMallocHost(&temp_storage, num_bytes));
       temp_storage_bytes = num_bytes;
     }
-    return xgboost::common::Span<T>(static_cast<T *>(temp_storage), size);
+    return boxhed_kernel::common::Span<T>(static_cast<T *>(temp_storage), size);
   }
 
   template <typename T>
-  xgboost::common::Span<T> GetSpan(size_t size, T init) {
+  boxhed_kernel::common::Span<T> GetSpan(size_t size, T init) {
     auto result = this->GetSpan<T>(size);
     for (auto &e : result) {
       e = init;
     }
     return result;
   }
 
@@ -796,68 +796,68 @@
         static_cast<int>(kRootRank));
     return id;
   }
 #endif
 };
 
 template <typename VectorT, typename T = typename VectorT::value_type,
-  typename IndexT = typename xgboost::common::Span<T>::index_type>
-xgboost::common::Span<T> ToSpan(
+  typename IndexT = typename boxhed_kernel::common::Span<T>::index_type>
+boxhed_kernel::common::Span<T> ToSpan(
     VectorT &vec,
     IndexT offset = 0,
     IndexT size = std::numeric_limits<size_t>::max()) {
   size = size == std::numeric_limits<size_t>::max() ? vec.size() : size;
   CHECK_LE(offset + size, vec.size());
   return {vec.data().get() + offset, size};
 }
 
 template <typename T>
-xgboost::common::Span<T> ToSpan(thrust::device_vector<T>& vec,
+boxhed_kernel::common::Span<T> ToSpan(thrust::device_vector<T>& vec,
                                 size_t offset, size_t size) {
   return ToSpan(vec, offset, size);
 }
 
 // thrust begin, similiar to std::begin
 template <typename T>
-thrust::device_ptr<T> tbegin(xgboost::HostDeviceVector<T>& vector) {  // NOLINT
+thrust::device_ptr<T> tbegin(boxhed_kernel::HostDeviceVector<T>& vector) {  // NOLINT
   return thrust::device_ptr<T>(vector.DevicePointer());
 }
 
 template <typename T>
-thrust::device_ptr<T> tend(xgboost::HostDeviceVector<T>& vector) {  // // NOLINT
+thrust::device_ptr<T> tend(boxhed_kernel::HostDeviceVector<T>& vector) {  // // NOLINT
   return tbegin(vector) + vector.Size();
 }
 
 template <typename T>
-thrust::device_ptr<T const> tcbegin(xgboost::HostDeviceVector<T> const& vector) {  // NOLINT
+thrust::device_ptr<T const> tcbegin(boxhed_kernel::HostDeviceVector<T> const& vector) {  // NOLINT
   return thrust::device_ptr<T const>(vector.ConstDevicePointer());
 }
 
 template <typename T>
-thrust::device_ptr<T const> tcend(xgboost::HostDeviceVector<T> const& vector) {  // NOLINT
+thrust::device_ptr<T const> tcend(boxhed_kernel::HostDeviceVector<T> const& vector) {  // NOLINT
   return tcbegin(vector) + vector.Size();
 }
 
 template <typename T>
-thrust::device_ptr<T> tbegin(xgboost::common::Span<T>& span) {  // NOLINT
+thrust::device_ptr<T> tbegin(boxhed_kernel::common::Span<T>& span) {  // NOLINT
   return thrust::device_ptr<T>(span.data());
 }
 
 template <typename T>
-thrust::device_ptr<T> tend(xgboost::common::Span<T>& span) {  // NOLINT
+thrust::device_ptr<T> tend(boxhed_kernel::common::Span<T>& span) {  // NOLINT
   return tbegin(span) + span.size();
 }
 
 template <typename T>
-thrust::device_ptr<T const> tcbegin(xgboost::common::Span<T> const& span) {  // NOLINT
+thrust::device_ptr<T const> tcbegin(boxhed_kernel::common::Span<T> const& span) {  // NOLINT
   return thrust::device_ptr<T const>(span.data());
 }
 
 template <typename T>
-thrust::device_ptr<T const> tcend(xgboost::common::Span<T> const& span) {  // NOLINT
+thrust::device_ptr<T const> tcend(boxhed_kernel::common::Span<T> const& span) {  // NOLINT
   return tcbegin(span) + span.size();
 }
 
 // This type sorts an array which is divided into multiple groups. The sorting is influenced
 // by the function object 'Comparator'
 template <typename T>
 class SegmentSorter {
@@ -914,32 +914,32 @@
                       thrust::make_counting_iterator(num_elems),
                       group_segments_.begin(),
                       ComputeGroupIDLambda);
   }
 
   // Accessors that returns device pointer
   inline uint32_t GetNumItems() const { return ditems_.size(); }
-  inline const xgboost::common::Span<const T> GetItemsSpan() const {
+  inline const boxhed_kernel::common::Span<const T> GetItemsSpan() const {
     return { ditems_.data().get(), ditems_.size() };
   }
 
-  inline const xgboost::common::Span<const uint32_t> GetOriginalPositionsSpan() const {
+  inline const boxhed_kernel::common::Span<const uint32_t> GetOriginalPositionsSpan() const {
     return { doriginal_pos_.data().get(), doriginal_pos_.size() };
   }
 
-  inline const xgboost::common::Span<const uint32_t> GetGroupSegmentsSpan() const {
+  inline const boxhed_kernel::common::Span<const uint32_t> GetGroupSegmentsSpan() const {
     return { group_segments_.data().get(), group_segments_.size() };
   }
 
   inline uint32_t GetNumGroups() const { return dgroups_.size() - 1; }
-  inline const xgboost::common::Span<const uint32_t> GetGroupsSpan() const {
+  inline const boxhed_kernel::common::Span<const uint32_t> GetGroupsSpan() const {
     return { dgroups_.data().get(), dgroups_.size() };
   }
 
-  inline const xgboost::common::Span<const uint32_t> GetIndexableSortedPositionsSpan() const {
+  inline const boxhed_kernel::common::Span<const uint32_t> GetIndexableSortedPositionsSpan() const {
     return { dindexable_sorted_pos_.data().get(), dindexable_sorted_pos_.size() };
   }
 
   // Sort an array that is divided into multiple groups. The array is sorted within each group.
   // This version provides the group information that is on the host.
   // The array is sorted based on an adaptable binary predicate. By default a stateless predicate
   // is used.
@@ -952,15 +952,15 @@
 
   // Sort an array that is divided into multiple groups. The array is sorted within each group.
   // This version provides the group information that is on the device.
   // The array is sorted based on an adaptable binary predicate. By default a stateless predicate
   // is used.
   template <typename Comparator = thrust::greater<T>>
   void SortItems(const T *ditems, uint32_t item_size,
-                 const xgboost::common::Span<const uint32_t> &group_segments,
+                 const boxhed_kernel::common::Span<const uint32_t> &group_segments,
                  const Comparator &comp = Comparator()) {
     this->Init(item_size);
 
     // Sort the items that are grouped. We would like to avoid using predicates to perform the sort,
     // as thrust resorts to using a merge sort as opposed to a much much faster radix sort
     // when comparators are used. Hence, the following algorithm is used. This is done so that
     // we can grab the appropriate related values from the original list later, after the
@@ -1051,15 +1051,15 @@
 size_t XGBOOST_DEVICE SegmentId(It first, It last, size_t idx) {
   size_t segment_id = thrust::upper_bound(thrust::seq, first, last, idx) -
                       1 - first;
   return segment_id;
 }
 
 template <typename T>
-size_t XGBOOST_DEVICE SegmentId(xgboost::common::Span<T> segments_ptr, size_t idx) {
+size_t XGBOOST_DEVICE SegmentId(boxhed_kernel::common::Span<T> segments_ptr, size_t idx) {
   return SegmentId(segments_ptr.cbegin(), segments_ptr.cend(), idx);
 }
 
 namespace detail {
 template <typename Key, typename KeyOutIt>
 struct SegmentedUniqueReduceOp {
   KeyOutIt key_out;
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/group_data.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/group_data.h`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 #define XGBOOST_COMMON_GROUP_DATA_H_
 
 #include <cstddef>
 #include <vector>
 #include <algorithm>
 #include <utility>
 
-#include "xgboost/base.h"
+#include "boxhed_kernel/base.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 /*!
  * \brief multi-thread version of group builder
  * \tparam ValueType type of entries in the sparse matrix
  * \tparam SizeType type of the index range holder
  */
 template<typename ValueType, typename SizeType = bst_ulong>
@@ -125,9 +125,9 @@
   std::vector<ValueType> &data_;
   /*! \brief thread local data structure */
   std::vector<std::vector<SizeType> > thread_rptr_;
   /** \brief Used when rows being pushed into the builder are strictly above some number. */
   size_t base_row_offset_;
 };
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_GROUP_DATA_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/hist_util.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/hist_util.cc`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #include <dmlc/timer.h>
 #include <dmlc/omp.h>
 
 #include <rabit/rabit.h>
 #include <numeric>
 #include <vector>
 
-#include "xgboost/base.h"
+#include "boxhed_kernel/base.h"
 #include "../common/common.h"
 #include "hist_util.h"
 #include "random.h"
 #include "column_matrix.h"
 #include "quantile.h"
 #include "./../tree/updater_quantile_hist.h"
 
@@ -22,15 +22,15 @@
   #define PREFETCH_READ_T0(addr) _mm_prefetch(reinterpret_cast<const char*>(addr), _MM_HINT_T0)
 #elif defined(XGBOOST_BUILTIN_PREFETCH_PRESENT)
   #define PREFETCH_READ_T0(addr) __builtin_prefetch(reinterpret_cast<const char*>(addr), 0, 3)
 #else  // no SW pre-fetching available; PREFETCH_READ_T0 is no-op
   #define PREFETCH_READ_T0(addr) do {} while (0)
 #endif  // defined(XGBOOST_MM_PREFETCH_PRESENT)
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 void GHistIndexMatrix::ResizeIndex(const size_t n_index,
                                    const bool isDense) {
   if ((max_num_bins - 1 <= static_cast<int>(std::numeric_limits<uint8_t>::max())) && isDense) {
     index.SetBinTypeSize(kUint8BinsTypeSize);
     index.Resize((sizeof(uint8_t)) * n_index);
@@ -180,15 +180,15 @@
 }
 
 template <typename BinIdxType>
 static size_t GetConflictCount(const std::vector<bool>& mark,
                                const Column<BinIdxType>& column_input,
                                size_t max_cnt) {
   size_t ret = 0;
-  if (column_input.GetType() == xgboost::common::kDenseColumn) {
+  if (column_input.GetType() == boxhed_kernel::common::kDenseColumn) {
     const DenseColumn<BinIdxType>& column
       = static_cast<const DenseColumn<BinIdxType>& >(column_input);
     for (size_t i = 0; i < column.Size(); ++i) {
       if ((!column.IsMissing(i)) && mark[i]) {
         ++ret;
         if (ret > max_cnt) {
           return max_cnt + 1;
@@ -210,15 +210,15 @@
   return ret;
 }
 
 template <typename BinIdxType>
 inline void
 MarkUsed(std::vector<bool>* p_mark, const Column<BinIdxType>& column_input) {
   std::vector<bool>& mark = *p_mark;
-  if (column_input.GetType() == xgboost::common::kDenseColumn) {
+  if (column_input.GetType() == boxhed_kernel::common::kDenseColumn) {
     const DenseColumn<BinIdxType>& column
       = static_cast<const DenseColumn<BinIdxType>& >(column_input);
     for (size_t i = 0; i < column.Size(); ++i) {
       if (!column.IsMissing(i)) {
         mark[i] = true;
       }
     }
@@ -443,18 +443,18 @@
 /*!
  * \brief fill a histogram by zeros in range [begin, end)
  */
 template<typename GradientSumT>
 void InitilizeHistByZeroes(GHistRow<GradientSumT> hist, size_t begin, size_t end) {
 #if defined(XGBOOST_STRICT_R_MODE) && XGBOOST_STRICT_R_MODE == 1
   std::fill(hist.begin() + begin, hist.begin() + end,
-            xgboost::detail::GradientPairInternal<GradientSumT>());
+            boxhed_kernel::detail::GradientPairInternal<GradientSumT>());
 #else  // defined(XGBOOST_STRICT_R_MODE) && XGBOOST_STRICT_R_MODE == 1
   memset(hist.data() + begin, '\0', (end-begin)*
-         sizeof(xgboost::detail::GradientPairInternal<GradientSumT>));
+         sizeof(boxhed_kernel::detail::GradientPairInternal<GradientSumT>));
 #endif  // defined(XGBOOST_STRICT_R_MODE) && XGBOOST_STRICT_R_MODE == 1
 }
 template void InitilizeHistByZeroes(GHistRow<float> hist, size_t begin,
                                     size_t end);
 template void InitilizeHistByZeroes(GHistRow<double> hist, size_t begin,
                                     size_t end);
 
@@ -703,15 +703,15 @@
   constexpr int kUnroll = 8;  // loop unrolling factor
   const size_t nblock = gmatb.GetNumBlock();
   const size_t nrows = row_indices.end - row_indices.begin;
   const size_t rest = nrows % kUnroll;
 #if defined(_OPENMP)
   const auto nthread = static_cast<bst_omp_uint>(this->nthread_);  // NOLINT
 #endif  // defined(_OPENMP)
-  xgboost::detail::GradientPairInternal<GradientSumT>* p_hist = hist.data();
+  boxhed_kernel::detail::GradientPairInternal<GradientSumT>* p_hist = hist.data();
 
 #pragma omp parallel for num_threads(nthread) schedule(guided)
   for (bst_omp_uint bid = 0; bid < nblock; ++bid) {
     auto gmat = gmatb[bid];
 
     for (size_t i = 0; i < nrows - rest; i += kUnroll) {
       size_t rid[kUnroll];
@@ -780,8 +780,8 @@
                                            GHistRow<float> parent);
 template
 void GHistBuilder<double>::SubtractionTrick(GHistRow<double> self,
                                             GHistRow<double> sibling,
                                             GHistRow<double> parent);
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/hist_util.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/hist_util.cu`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 /*!
  * Copyright 2018~2020 XGBoost contributors
  */
 
-#include <xgboost/logging.h>
+#include <boxhed_kernel/logging.h>
 
 #include <thrust/copy.h>
 #include <thrust/functional.h>
 #include <thrust/iterator/counting_iterator.h>
 #include <thrust/iterator/transform_iterator.h>
 #include <thrust/iterator/discard_iterator.h>
 #include <thrust/reduce.h>
@@ -21,18 +21,18 @@
 
 #include "device_helpers.cuh"
 #include "hist_util.h"
 #include "hist_util.cuh"
 #include "math.h"  // NOLINT
 #include "quantile.h"
 #include "categorical.h"
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/host_device_vector.h"
 
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 constexpr float SketchContainer::kFactor;
 
 namespace detail {
 size_t RequiredSampleCutsPerColumn(int max_bins, size_t num_rows) {
   double eps = 1.0 / (WQSketch::kFactor * max_bins);
@@ -446,8 +446,8 @@
       }
     }
   }
   sketch_container.MakeCuts(&cuts);
   return cuts;
 }
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/hist_util.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/hist_util.cuh`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 #include "hist_util.h"
 #include "quantile.cuh"
 #include "device_helpers.cuh"
 #include "timer.h"
 #include "../data/device_adapter.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 namespace detail {
 struct EntryCompareOp {
   __device__ bool operator()(const Entry& a, const Entry& b) {
     if (a.index == b.index) {
       return a.fvalue < b.fvalue;
@@ -290,10 +290,10 @@
       size_t end = std::min(batch.Size(), size_t(begin + sketch_batch_num_elements));
       ProcessSlidingWindow(batch, device, num_cols,
                            begin, end, missing, sketch_container, num_cuts_per_feature);
     }
   }
 }
 }      // namespace common
-}      // namespace xgboost
+}      // namespace boxhed_kernel
 
 #endif  // COMMON_HIST_UTIL_CUH_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/hist_util.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/hist_util.h`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
  * \file hist_util.h
  * \brief Utility for fast histogram aggregation
  * \author Philip Cho, Tianqi Chen
  */
 #ifndef XGBOOST_COMMON_HIST_UTIL_H_
 #define XGBOOST_COMMON_HIST_UTIL_H_
 
-#include <xgboost/data.h>
-#include <xgboost/generic_parameters.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/generic_parameters.h>
 #include <limits>
 #include <vector>
 #include <algorithm>
 #include <memory>
 #include <utility>
 #include <map>
 
@@ -20,15 +20,15 @@
 #include "common.h"
 #include "threading_utils.h"
 #include "../tree/param.h"
 #include "./quantile.h"
 #include "./timer.h"
 #include "../include/rabit/rabit.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 /*!
  * \brief A single row in global histogram index.
  *  Directly represent the global index in the histogram entry.
  */
 using GHistIndexRow = Span<uint32_t const>;
 
@@ -248,15 +248,15 @@
   void Init(DMatrix* p_fmat, int max_num_bins);
 
   // specific method for sparse data as no posibility to reduce allocated memory
   template <typename BinIdxType, typename GetOffset>
   void SetIndexData(common::Span<BinIdxType> index_data_span,
                     size_t batch_threads, const SparsePage &batch,
                     size_t rbegin, size_t nbins, GetOffset get_offset) {
-    const xgboost::Entry *data_ptr = batch.data.HostVector().data();
+    const boxhed_kernel::Entry *data_ptr = batch.data.HostVector().data();
     const std::vector<bst_row_t> &offset_vec = batch.offset.HostVector();
     const size_t batch_size = batch.Size();
     CHECK_LT(batch_size, offset_vec.size());
     BinIdxType* index_data = index_data_span.data();
 #pragma omp parallel for num_threads(batch_threads) schedule(static)
     for (omp_ulong i = 0; i < batch_size; ++i) {
       const int tid = omp_get_thread_num();
@@ -361,15 +361,15 @@
     const uint32_t* index_begin;
     const uint32_t* index_end;
   };
   std::vector<Block> blocks_;
 };
 
 template<typename GradientSumT>
-using GHistRow = Span<xgboost::detail::GradientPairInternal<GradientSumT> >;
+using GHistRow = Span<boxhed_kernel::detail::GradientPairInternal<GradientSumT> >;
 
 /*!
  * \brief fill a histogram by zeros
  */
 template<typename GradientSumT>
 void InitilizeHistByZeroes(GHistRow<GradientSumT> hist, size_t begin, size_t end);
 
@@ -398,15 +398,15 @@
 /*!
  * \brief histogram of gradient statistics for multiple nodes
  */
 template<typename GradientSumT>
 class HistCollection {
  public:
   using GHistRowT = GHistRow<GradientSumT>;
-  using GradientPairT = xgboost::detail::GradientPairInternal<GradientSumT>;
+  using GradientPairT = boxhed_kernel::detail::GradientPairInternal<GradientSumT>;
 
   // access histogram for i-th node
   GHistRowT operator[](bst_uint nid) const {
     constexpr uint32_t kMax = std::numeric_limits<uint32_t>::max();
     CHECK_NE(row_ptr_[nid], kMax);
     GradientPairT* ptr =
         const_cast<GradientPairT*>(dmlc::BeginPtr(data_) + row_ptr_[nid]);
@@ -670,9 +670,9 @@
  private:
   /*! \brief number of threads for parallel computation */
   size_t nthread_ { 0 };
   /*! \brief number of all bins over all features */
   uint32_t nbins_ { 0 };
 };
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_HIST_UTIL_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/host_device_vector.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/host_device_vector.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 /*!
  * Copyright 2017 XGBoost contributors
  */
 #ifndef XGBOOST_USE_CUDA
 
 // dummy implementation of HostDeviceVector in case CUDA is not used
 
-#include <xgboost/base.h>
-#include <xgboost/data.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/data.h>
 #include <cstdint>
 #include <memory>
 #include <utility>
-#include "xgboost/tree_model.h"
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/tree_model.h"
+#include "boxhed_kernel/host_device_vector.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 template <typename T>
 struct HostDeviceVectorImpl {
   explicit HostDeviceVectorImpl(size_t size, T v) : data_h_(size, v) {}
   HostDeviceVectorImpl(std::initializer_list<T> init) : data_h_(init) {}
   explicit HostDeviceVectorImpl(std::vector<T>  init) : data_h_(std::move(init)) {}
   HostDeviceVectorImpl(HostDeviceVectorImpl&& that) : data_h_(std::move(that.data_h_)) {}
@@ -186,10 +186,10 @@
  * typedef unsigned int         uint32_t;
  * typedef unsigned long long   uint64_t;
  * typedef unsigned long       __darwin_size_t;
  */
 template class HostDeviceVector<std::size_t>;
 #endif  // defined(__APPLE__)
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_USE_CUDA
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/host_device_vector.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/host_device_vector.cu`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 #include <thrust/fill.h>
 #include <thrust/device_ptr.h>
 
 #include <algorithm>
 #include <cstdint>
 #include <mutex>
 
-#include "xgboost/data.h"
-#include "xgboost/host_device_vector.h"
-#include "xgboost/tree_model.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/tree_model.h"
 #include "device_helpers.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 // the handler to call instead of cudaSetDevice; only used for testing
 static void (*cudaSetDeviceHandler)(int) = nullptr;  // NOLINT
 
 void SetCudaSetDeviceHandler(void (*handler)(int)) {
   cudaSetDeviceHandler = handler;
 }
@@ -414,8 +414,8 @@
  * typedef unsigned int         uint32_t;
  * typedef unsigned long long   uint64_t;
  * typedef unsigned long       __darwin_size_t;
  */
 template class HostDeviceVector<std::size_t>;
 #endif  // defined(__APPLE__)
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/io.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/io.cc`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 #include <algorithm>
 #include <fstream>
 #include <string>
 #include <memory>
 #include <utility>
 #include <cstdio>
 
-#include "xgboost/logging.h"
+#include "boxhed_kernel/logging.h"
 #include "io.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 size_t PeekableInStream::Read(void* dptr, size_t size) {
   size_t nbuffer = buffer_.length() - buffer_ptr_;
   if (nbuffer == 0) return strm_->Read(dptr, size);
   if (nbuffer < size) {
     std::memcpy(dptr, dmlc::BeginPtr(buffer_) + buffer_ptr_, nbuffer);
@@ -139,8 +139,8 @@
     }
     size *= 2;
   }
   buffer.resize(total);
   return buffer;
 }
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/io.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/io.h`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #include <dmlc/io.h>
 #include <rabit/rabit.h>
 #include <string>
 #include <cstring>
 
 #include "common.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 using MemoryFixSizeBuffer = rabit::utils::MemoryFixSizeBuffer;
 using MemoryBufferStream = rabit::utils::MemoryBufferStream;
 
 /*!
  * \brief Input stream that support additional PeekRead operation,
  *  besides read.
@@ -92,9 +92,9 @@
     return splited.back();
   } else {
     return "";
   }
 }
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_IO_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/json.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/json.cc`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 #include <iterator>
 #include <locale>
 #include <sstream>
 #include <limits>
 #include <cmath>
 
 #include "charconv.h"
-#include "xgboost/base.h"
-#include "xgboost/logging.h"
-#include "xgboost/json.h"
-#include "xgboost/json_io.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/json_io.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 void JsonWriter::Save(Json json) {
   json.ptr_->Save(this);
 }
 
 void JsonWriter::Visit(JsonArray const* arr) {
   stream_->emplace_back('[');
@@ -740,8 +740,8 @@
   JsonWriter writer(&buffer);
   writer.Save(json);
   str->resize(buffer.size());
   std::copy(buffer.cbegin(), buffer.cend(), str->begin());
 }
 
 Json& Json::operator=(Json const &other) = default;
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/math.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/math.h`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
  * \file math.h
  * \brief additional math utils
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_COMMON_MATH_H_
 #define XGBOOST_COMMON_MATH_H_
 
-#include <xgboost/base.h>
+#include <boxhed_kernel/base.h>
 
 #include <algorithm>
 #include <cmath>
 #include <limits>
 #include <utility>
 #include <vector>
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 /*!
  * \brief calculate the sigmoid of the input.
  * \param x input parameter
  * \return the transformed value.
  */
 XGBOOST_DEVICE inline float Sigmoid(float x) {
@@ -188,9 +188,9 @@
   return lgamma(v);
 #endif  // _MSC_VER
 }
 
 #endif  // XGBOOST_STRICT_R_MODE && !defined(XGBOOST_USE_CUDA)
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_MATH_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/observer.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/observer.h`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 
 #include <iostream>
 #include <algorithm>
 #include <limits>
 #include <string>
 #include <vector>
 
-#include "xgboost/host_device_vector.h"
-#include "xgboost/parameter.h"
-#include "xgboost/json.h"
-#include "xgboost/base.h"
-#include "xgboost/tree_model.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/tree_model.h"
 
 #if defined(XGBOOST_STRICT_R_MODE) && XGBOOST_STRICT_R_MODE == 1
 #define OBSERVER_PRINT LOG(INFO)
 #define OBSERVER_ENDL ""
 #define OBSERVER_NEWLINE ""
 #else  // defined(XGBOOST_STRICT_R_MODE) && XGBOOST_STRICT_R_MODE == 1
 #define OBSERVER_PRINT std::cout << std::setprecision(17)
 #define OBSERVER_ENDL std::endl
 #define OBSERVER_NEWLINE "\n"
 #endif  // defined(XGBOOST_STRICT_R_MODE) && XGBOOST_STRICT_R_MODE == 1
 
-namespace xgboost {
+namespace boxhed_kernel {
 /*\brief  An observer for logging internal data structures.
  *
  *  This class is designed to be `diff` tool friendly, which means it uses plain
  *  `std::cout` for printing to avoid the time information emitted by `LOG(DEBUG)` or
  *  similiar facilities. Exception: use `LOG(INFO)` for the R package, to comply
  *  with CRAN policy.
  */
@@ -125,9 +125,9 @@
 
   /*\brief Get a global instance. */
   static TrainingObserver& Instance() {
     static TrainingObserver observer;
     return observer;
   }
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_OBSERVER_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/probability_distribution.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/probability_distribution.h`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  */
 
 #ifndef XGBOOST_COMMON_PROBABILITY_DISTRIBUTION_H_
 #define XGBOOST_COMMON_PROBABILITY_DISTRIBUTION_H_
 
 #include <cmath>
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 #ifndef __CUDACC__
 
 using std::exp;
 using std::sqrt;
 using std::isinf;
@@ -116,10 +116,10 @@
 
   XGBOOST_DEVICE static ProbabilityDistributionType Type() {
     return ProbabilityDistributionType::kExtreme;
   }
 };
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_COMMON_PROBABILITY_DISTRIBUTION_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/quantile.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/quantile.cc`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  * Copyright 2020 by XGBoost Contributors
  */
 #include <limits>
 #include <utility>
 #include "quantile.h"
 #include "hist_util.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 HostSketchContainer::HostSketchContainer(std::vector<bst_row_t> columns_size,
                                          int32_t max_bins, bool use_group)
     : columns_size_{std::move(columns_size)}, max_bins_{max_bins},
       use_group_ind_{use_group} {
   monitor_.Init(__func__);
@@ -319,8 +319,8 @@
     auto cut_size = static_cast<uint32_t>(cuts->cut_values_.HostVector().size());
     CHECK_GT(cut_size, cuts->cut_ptrs_.HostVector().back());
     cuts->cut_ptrs_.HostVector().push_back(cut_size);
   }
   monitor_.Stop(__func__);
 }
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/quantile.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/quantile.cu`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 #include <thrust/binary_search.h>
 #include <thrust/transform_scan.h>
 #include <thrust/execution_policy.h>
 
 #include <memory>
 #include <utility>
 
-#include "xgboost/span.h"
+#include "boxhed_kernel/span.h"
 #include "quantile.h"
 #include "quantile.cuh"
 #include "hist_util.h"
 #include "device_helpers.cuh"
 #include "categorical.h"
 #include "common.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 using WQSketch = HostSketchContainer::WQSketch;
 using SketchEntry = WQSketch::Entry;
 
 // Algorithm 4 in XGBoost's paper, using binary search to find i.
 template <typename EntryIter>
@@ -733,8 +733,8 @@
     }
     assert(idx+1 < in_column.size());
     out_column[idx] = in_column[idx+1].value;
   });
   timer_.Stop(__func__);
 }
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/quantile.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/quantile.cuh`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #ifndef XGBOOST_COMMON_QUANTILE_CUH_
 #define XGBOOST_COMMON_QUANTILE_CUH_
 
 #include <memory>
 
-#include "xgboost/span.h"
-#include "xgboost/data.h"
+#include "boxhed_kernel/span.h"
+#include "boxhed_kernel/data.h"
 #include "device_helpers.cuh"
 #include "quantile.h"
 #include "timer.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 class HistogramCuts;
 using WQSketch = WQuantileSketch<bst_float, bst_float>;
 using SketchEntry = WQSketch::Entry;
 
 /*!
@@ -161,10 +161,10 @@
 struct SketchUnique {
   XGBOOST_DEVICE bool operator()(SketchEntry const& a, SketchEntry const& b) const {
     return a.value - b.value == 0;
   }
 };
 }  // namespace detail
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_COMMON_QUANTILE_CUH_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/quantile.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/quantile.h`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
  * \brief util to compute quantiles
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_COMMON_QUANTILE_H_
 #define XGBOOST_COMMON_QUANTILE_H_
 
 #include <dmlc/base.h>
-#include <xgboost/logging.h>
-#include <xgboost/data.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/data.h>
 #include <cmath>
 #include <vector>
 #include <cstring>
 #include <algorithm>
 #include <iostream>
 
 #include "timer.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 /*!
  * \brief experimental wsummary
  * \tparam DType type of data content
  * \tparam RType type of rank
  */
 template<typename DType, typename RType>
@@ -759,9 +759,9 @@
 
   /* \brief Push a CSR matrix. */
   void PushRowPage(SparsePage const& page, MetaInfo const& info);
 
   void MakeCuts(HistogramCuts* cuts);
 };
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_QUANTILE_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/random.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/random.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*!
  * Copyright 2020 by XGBoost Contributors
  * \file random.cc
  */
 #include "random.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 std::shared_ptr<HostDeviceVector<bst_feature_t>> ColumnSampler::ColSample(
     std::shared_ptr<HostDeviceVector<bst_feature_t>> p_features,
     float colsample) {
   if (colsample == 1.0f) {
     return p_features;
   }
@@ -31,8 +31,8 @@
     new_features.Resize(n);
   }
   std::sort(new_features.HostVector().begin(), new_features.HostVector().end());
   return p_new_features;
 }
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/random.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/random.h`

 * *Files 10% similar despite different names*

```diff
@@ -4,39 +4,39 @@
  * \brief Utility related to random.
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_COMMON_RANDOM_H_
 #define XGBOOST_COMMON_RANDOM_H_
 
 #include <rabit/rabit.h>
-#include <xgboost/logging.h>
+#include <boxhed_kernel/logging.h>
 #include <algorithm>
 #include <functional>
 #include <vector>
 #include <limits>
 #include <map>
 #include <memory>
 #include <numeric>
 #include <random>
 #include <utility>
 
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/host_device_vector.h"
 #include "common.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 /*!
  * \brief Define mt19937 as default type Random Engine.
  */
 using RandomEngine = std::mt19937;
 
 #if XGBOOST_CUSTOMIZE_GLOBAL_PRNG
 /*!
  * \brief An customized random engine, used to be plugged in PRNG from other systems.
- *  The implementation of this library is not provided by xgboost core library.
+ *  The implementation of this library is not provided by boxhed_kernel core library.
  *  Instead the other library can implement this class, which will be used as GlobalRandomEngine
  *  If XGBOOST_RANDOM_CUSTOMIZE = 1, by default this is switched off.
  */
 class CustomGlobalRandomEngine {
  public:
   /*! \brief The result type */
   using result_type = uint32_t;
@@ -188,15 +188,15 @@
   /**
    * \brief Samples a feature set.
    *
    * \param depth The tree depth of the node at which to sample.
    * \return The sampled feature set.
    * \note If colsample_bynode_ < 1.0, this method creates a new feature set each time it
    * is called. Therefore, it should be called only once per node.
-   * \note With distributed xgboost, this function must be called exactly once for the
+   * \note With distributed boxhed_kernel, this function must be called exactly once for the
    * construction of each tree node, and must be called the same number of times in each
    * process and with the same parameters to return the same feature set across processes.
    */
   std::shared_ptr<HostDeviceVector<bst_feature_t>> GetFeatureSet(int depth) {
     if (colsample_bylevel_ == 1.0f && colsample_bynode_ == 1.0f) {
       return feature_set_tree_;
     }
@@ -211,9 +211,9 @@
     }
     // Need to sample for the node individually
     return ColSample(feature_set_level_[depth], colsample_bynode_);
   }
 };
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_RANDOM_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/row_set.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/row_set.h`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
  * \file row_set.h
  * \brief Quick Utility to compute subset of rows
  * \author Philip Cho, Tianqi Chen
  */
 #ifndef XGBOOST_COMMON_ROW_SET_H_
 #define XGBOOST_COMMON_ROW_SET_H_
 
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 #include <algorithm>
 #include <vector>
 #include <utility>
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 /*! \brief collection of rowset */
 class RowSetCollection {
  public:
   /*! \brief data structure to store an instance set, a subset of
    *  rows (instances) associated with a particular node in a decision
@@ -237,10 +237,10 @@
   std::vector<size_t> blocks_offsets_;
   std::vector<BlockInfo> mem_blocks_;
   size_t max_n_tasks_ = 0;
 };
 
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_COMMON_ROW_SET_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/survival_util.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/survival_util.h`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 /*
  * For the derivation of the loss, gradient, and hessian for the Accelerated Failure Time model,
  * refer to the paper "Survival regression with accelerated failure time model in XGBoost"
  * at https://arxiv.org/abs/2006.04920.
  */
 
-#include <xgboost/parameter.h>
+#include <boxhed_kernel/parameter.h>
 #include <memory>
 #include <algorithm>
 #include <limits>
 #include "probability_distribution.h"
 
-DECLARE_FIELD_ENUM_CLASS(xgboost::common::ProbabilityDistributionType);
+DECLARE_FIELD_ENUM_CLASS(boxhed_kernel::common::ProbabilityDistributionType);
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 #ifndef __CUDACC__
 
 using std::log;
 using std::fmax;
 
@@ -338,10 +338,10 @@
   }
   return std::numeric_limits<double>::quiet_NaN();
 }
 
 }  // namespace aft
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_COMMON_SURVIVAL_UTIL_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/threading_utils.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/threading_utils.h`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
  */
 #ifndef XGBOOST_COMMON_THREADING_UTILS_H_
 #define XGBOOST_COMMON_THREADING_UTILS_H_
 
 #include <dmlc/common.h>
 #include <vector>
 #include <algorithm>
-#include "xgboost/logging.h"
+#include "boxhed_kernel/logging.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 // Represent simple range of indexes [begin, end)
 // Inspired by tbb::blocked_range
 class Range1d {
  public:
   Range1d(size_t begin, size_t end): begin_(begin), end_(end) {
@@ -167,10 +167,10 @@
     threads = nthread_original;
   }
   omp_set_num_threads(threads);
   return nthread_original;
 }
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_COMMON_THREADING_UTILS_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/timer.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/timer.cc`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 #include <rabit/rabit.h>
 #include <algorithm>
 #include <type_traits>
 #include <utility>
 #include <vector>
 #include <sstream>
 #include "timer.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/json.h"
 
 #if defined(XGBOOST_USE_NVTX)
 #include <nvToolsExt.h>
 #endif  // defined(XGBOOST_USE_NVTX)
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 void Monitor::Start(std::string const &name) {
   if (ConsoleLogger::ShouldLog(ConsoleLogger::LV::kDebug)) {
     auto &stats = statistics_map_[name];
     stats.timer.Start();
 #if defined(XGBOOST_USE_NVTX)
@@ -132,8 +132,8 @@
     }
     LOG(CONSOLE) << "======== Monitor: " << label_ << " ========";
     this->PrintStatistics(stat_map);
   }
 }
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/timer.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/timer.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 /*!
  * Copyright by Contributors 2017-2019
  */
 #pragma once
-#include <xgboost/logging.h>
+#include <boxhed_kernel/logging.h>
 #include <chrono>
 #include <iostream>
 #include <map>
 #include <string>
 #include <utility>
 #include <vector>
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 struct Timer {
   using ClockT = std::chrono::high_resolution_clock;
   using TimePointT = std::chrono::high_resolution_clock::time_point;
   using DurationT = std::chrono::high_resolution_clock::duration;
   using SecondsT = std::chrono::duration<double>;
@@ -80,8 +80,8 @@
   void Print() const;
 
   void Init(std::string label) { this->label_ = label; }
   void Start(const std::string &name);
   void Stop(const std::string &name);
 };
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/transform.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/transform.h`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,29 @@
  */
 #ifndef XGBOOST_COMMON_TRANSFORM_H_
 #define XGBOOST_COMMON_TRANSFORM_H_
 
 #include <dmlc/omp.h>
 #include <dmlc/common.h>
 
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 #include <utility>
 #include <vector>
 #include <type_traits>  // enable_if
 
-#include "xgboost/host_device_vector.h"
-#include "xgboost/span.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/span.h"
 
 #include "common.h"
 
 #if defined (__CUDACC__)
 #include "device_helpers.cuh"
 #endif  // defined (__CUDACC__)
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace common {
 
 constexpr size_t kBlockThreads = 256;
 
 namespace detail {
 
 #if defined(__CUDACC__)
@@ -205,10 +205,10 @@
                                  int device,
                                  bool const shard = true) {
     return Evaluator<Functor> {func, std::move(range), device, shard};
   }
 };
 
 }  // namespace common
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_COMMON_TRANSFORM_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/version.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/version.cc`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
  */
 #include <dmlc/io.h>
 
 #include <string>
 #include <tuple>
 #include <vector>
 
-#include "xgboost/logging.h"
-#include "xgboost/json.h"
-#include "xgboost/version_config.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/version_config.h"
 #include "version.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 const Version::TripletT Version::kInvalid {-1, -1, -1};
 
 Version::TripletT Version::Load(Json const& in) {
   if (get<Object const>(in).find("version") == get<Object const>(in).cend()) {
     return kInvalid;
   }
@@ -84,8 +84,8 @@
   return std::make_tuple(XGBOOST_VER_MAJOR, XGBOOST_VER_MINOR, XGBOOST_VER_PATCH);
 }
 
 bool Version::Same(TripletT const& triplet) {
   return triplet == Self();
 }
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/common/version.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/common/version.h`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #ifndef XGBOOST_COMMON_VERSION_H_
 #define XGBOOST_COMMON_VERSION_H_
 
 #include <dmlc/io.h>
 #include <string>
 #include <tuple>
 
-#include "xgboost/base.h"
+#include "boxhed_kernel/base.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 class Json;
 // a static class for handling version info
 struct Version {
   using TripletT = std::tuple<XGBoostVersionT, XGBoostVersionT, XGBoostVersionT>;
   static const TripletT kInvalid;
 
   // Save/Load version info to Json document
@@ -27,9 +27,9 @@
 
   static std::string String(TripletT const& version);
   static TripletT Self();
 
   static bool Same(TripletT const& triplet);
 };
 
-}      // namespace xgboost
+}      // namespace boxhed_kernel
 #endif  // XGBOOST_COMMON_VERSION_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/adapter.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/adapter.h`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 #include <functional>
 #include <limits>
 #include <memory>
 #include <string>
 #include <utility>
 #include <vector>
 
-#include "xgboost/logging.h"
-#include "xgboost/base.h"
-#include "xgboost/data.h"
-#include "xgboost/span.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/span.h"
 
 #include "array_interface.h"
 #include "../c_api/c_api_error.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 /**  External data formats should implement an adapter as below. The
- * adapter provides a uniform access to data outside xgboost, allowing
+ * adapter provides a uniform access to data outside boxhed_kernel, allowing
  * construction of DMatrix objects from a range of sources without duplicating
  * code.
  *
  * The adapter object is an iterator that returns batches of data. Each batch
  * contains a number of "lines". A line represents a set of elements from a
  * sparse input matrix, normally a row in the case of a CSR matrix or a column
  * for a CSC matrix. Typically in sparse matrix formats we can efficiently
@@ -596,9 +596,9 @@
   // call back to get the data.
   XGBCallbackDataIterNext *next_callback_;
   // internal Rowblock
   dmlc::RowBlock<uint32_t> block_;
   std::unique_ptr<FileAdapterBatch> batch_;
 };
 };  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_DATA_ADAPTER_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/array_interface.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/array_interface.h`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 #define XGBOOST_DATA_ARRAY_INTERFACE_H_
 
 #include <cinttypes>
 #include <map>
 #include <string>
 #include <utility>
 
-#include "xgboost/base.h"
-#include "xgboost/data.h"
-#include "xgboost/json.h"
-#include "xgboost/logging.h"
-#include "xgboost/span.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/span.h"
 #include "../common/bitfield.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 // Common errors in parsing columnar format.
 struct ArrayInterfaceErrors {
   static char const* Contigious() {
     return "Memory should be contigious.";
   }
   static char const* TypestrFormat() {
     return "`typestr' should be of format <endian><type><size of type in bytes>.";
@@ -342,9 +342,9 @@
   RBitField8 valid;
   bst_row_t num_rows;
   bst_feature_t num_cols;
   void* data;
   char type[3];
 };
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_DATA_ARRAY_INTERFACE_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/data.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/data.cc`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,20 @@
  * Copyright 2015-2020 by Contributors
  * \file data.cc
  */
 #include <dmlc/registry.h>
 #include <cstring>
 
 #include "dmlc/io.h"
-#include "xgboost/data.h"
-#include "xgboost/c_api.h"
-#include "xgboost/host_device_vector.h"
-#include "xgboost/logging.h"
-#include "xgboost/version_config.h"
-#include "xgboost/learner.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/c_api.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/version_config.h"
+#include "boxhed_kernel/learner.h"
 #include "sparse_page_writer.h"
 #include "simple_dmatrix.h"
 
 #include "../common/io.h"
 #include "../common/math.h"
 #include "../common/version.h"
 #include "../common/group_data.h"
@@ -25,85 +25,85 @@
 
 #if DMLC_ENABLE_STD_THREAD
 #include "./sparse_page_source.h"
 #include "./sparse_page_dmatrix.h"
 #endif  // DMLC_ENABLE_STD_THREAD
 
 namespace dmlc {
-DMLC_REGISTRY_ENABLE(::xgboost::data::SparsePageFormatReg<::xgboost::SparsePage>);
-DMLC_REGISTRY_ENABLE(::xgboost::data::SparsePageFormatReg<::xgboost::CSCPage>);
-DMLC_REGISTRY_ENABLE(::xgboost::data::SparsePageFormatReg<::xgboost::SortedCSCPage>);
-DMLC_REGISTRY_ENABLE(::xgboost::data::SparsePageFormatReg<::xgboost::EllpackPage>);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::data::SparsePageFormatReg<::boxhed_kernel::SparsePage>);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::data::SparsePageFormatReg<::boxhed_kernel::CSCPage>);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::data::SparsePageFormatReg<::boxhed_kernel::SortedCSCPage>);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::data::SparsePageFormatReg<::boxhed_kernel::EllpackPage>);
 }  // namespace dmlc
 
 namespace {
 
 template <typename T>
 void SaveScalarField(dmlc::Stream *strm, const std::string &name,
-                     xgboost::DataType type, const T &field) {
+                     boxhed_kernel::DataType type, const T &field) {
   strm->Write(name);
   strm->Write(static_cast<uint8_t>(type));
   strm->Write(true);  // is_scalar=True
   strm->Write(field);
 }
 
 template <typename T>
 void SaveVectorField(dmlc::Stream *strm, const std::string &name,
-                     xgboost::DataType type, std::pair<uint64_t, uint64_t> shape,
+                     boxhed_kernel::DataType type, std::pair<uint64_t, uint64_t> shape,
                      const std::vector<T>& field) {
   strm->Write(name);
   strm->Write(static_cast<uint8_t>(type));
   strm->Write(false);  // is_scalar=False
   strm->Write(shape.first);
   strm->Write(shape.second);
   strm->Write(field);
 }
 
 template <typename T>
 void SaveVectorField(dmlc::Stream* strm, const std::string& name,
-                     xgboost::DataType type, std::pair<uint64_t, uint64_t> shape,
-                     const xgboost::HostDeviceVector<T>& field) {
+                     boxhed_kernel::DataType type, std::pair<uint64_t, uint64_t> shape,
+                     const boxhed_kernel::HostDeviceVector<T>& field) {
   SaveVectorField(strm, name, type, shape, field.ConstHostVector());
 }
 
 template <typename T>
 void LoadScalarField(dmlc::Stream* strm, const std::string& expected_name,
-                     xgboost::DataType expected_type, T* field) {
+                     boxhed_kernel::DataType expected_type, T* field) {
   const std::string invalid {"MetaInfo: Invalid format. "};
   std::string name;
-  xgboost::DataType type;
+  boxhed_kernel::DataType type;
   bool is_scalar;
   CHECK(strm->Read(&name)) << invalid;
   CHECK_EQ(name, expected_name)
       << invalid << " Expected field: " << expected_name << ", got: " << name;
   uint8_t type_val;
   CHECK(strm->Read(&type_val)) << invalid;
-  type = static_cast<xgboost::DataType>(type_val);
+  type = static_cast<boxhed_kernel::DataType>(type_val);
   CHECK(type == expected_type)
       << invalid << "Expected field of type: " << static_cast<int>(expected_type) << ", "
       << "got field type: " << static_cast<int>(type);
   CHECK(strm->Read(&is_scalar)) << invalid;
   CHECK(is_scalar)
     << invalid << "Expected field " << expected_name << " to be a scalar; got a vector";
   CHECK(strm->Read(field)) << invalid;
 }
 
 template <typename T>
 void LoadVectorField(dmlc::Stream* strm, const std::string& expected_name,
-                     xgboost::DataType expected_type, std::vector<T>* field) {
+                     boxhed_kernel::DataType expected_type, std::vector<T>* field) {
   const std::string invalid {"MetaInfo: Invalid format. "};
   std::string name;
-  xgboost::DataType type;
+  boxhed_kernel::DataType type;
   bool is_scalar;
   CHECK(strm->Read(&name)) << invalid;
   CHECK_EQ(name, expected_name)
     << invalid << " Expected field: " << expected_name << ", got: " << name;
   uint8_t type_val;
   CHECK(strm->Read(&type_val)) << invalid;
-  type = static_cast<xgboost::DataType>(type_val);
+  type = static_cast<boxhed_kernel::DataType>(type_val);
   CHECK(type == expected_type)
     << invalid << "Expected field of type: " << static_cast<int>(expected_type) << ", "
     << "got field type: " << static_cast<int>(type);
   CHECK(strm->Read(&is_scalar)) << invalid;
   CHECK(!is_scalar)
     << invalid << "Expected field " << expected_name << " to be a vector; got a scalar";
   std::pair<uint64_t, uint64_t> shape;
@@ -114,22 +114,22 @@
   CHECK_EQ(shape.second, 1) << invalid << "Number of columns is expected to be 1.";
 
   CHECK(strm->Read(field)) << invalid;
 }
 
 template <typename T>
 void LoadVectorField(dmlc::Stream* strm, const std::string& expected_name,
-                     xgboost::DataType expected_type,
-                     xgboost::HostDeviceVector<T>* field) {
+                     boxhed_kernel::DataType expected_type,
+                     boxhed_kernel::HostDeviceVector<T>* field) {
   LoadVectorField(strm, expected_name, expected_type, &field->HostVector());
 }
 
 }  // anonymous namespace
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 uint64_t constexpr MetaInfo::kNumField;
 
 // implementation of inline functions
 void MetaInfo::Clear() {
   num_row_ = num_col_ = num_nonzero_ = 0;
   labels_.HostVector().clear();
@@ -330,24 +330,24 @@
   }
   return true;
 }
 
 // macro to dispatch according to specified pointer types
 #define DISPATCH_CONST_PTR(dtype, old_ptr, cast_ptr, proc)              \
   switch (dtype) {                                                      \
-    case xgboost::DataType::kFloat32: {                                 \
+    case boxhed_kernel::DataType::kFloat32: {                                 \
       auto cast_ptr = reinterpret_cast<const float*>(old_ptr); proc; break; \
     }                                                                   \
-    case xgboost::DataType::kDouble: {                                  \
+    case boxhed_kernel::DataType::kDouble: {                                  \
       auto cast_ptr = reinterpret_cast<const double*>(old_ptr); proc; break; \
     }                                                                   \
-    case xgboost::DataType::kUInt32: {                                  \
+    case boxhed_kernel::DataType::kUInt32: {                                  \
       auto cast_ptr = reinterpret_cast<const uint32_t*>(old_ptr); proc; break; \
     }                                                                   \
-    case xgboost::DataType::kUInt64: {                                  \
+    case boxhed_kernel::DataType::kUInt64: {                                  \
       auto cast_ptr = reinterpret_cast<const uint64_t*>(old_ptr); proc; break; \
     }                                                                   \
     default: LOG(FATAL) << "Unknown data type" << static_cast<uint8_t>(dtype); \
   }                                                                     \
 
 void MetaInfo::SetInfo(const char* key, const void* dptr, DataType dtype, size_t num) {
   if (!std::strcmp(key, "label")) {
@@ -416,24 +416,24 @@
     } else if (!std::strcmp(key, "label_upper_bound")) {
       vec = &this->labels_upper_bound_.HostVector();
     } else if (!std::strcmp(key, "feature_weights")) {
       vec = &this->feature_weigths.HostVector();
     } else {
       LOG(FATAL) << "Unknown float field name: " << key;
     }
-    *out_len = static_cast<xgboost::bst_ulong>(vec->size()); // NOLINT
+    *out_len = static_cast<boxhed_kernel::bst_ulong>(vec->size()); // NOLINT
     *reinterpret_cast<float const**>(out_dptr) = dmlc::BeginPtr(*vec);
   } else if (dtype == DataType::kUInt32) {
     const std::vector<unsigned> *vec = nullptr;
     if (!std::strcmp(key, "group_ptr")) {
       vec = &this->group_ptr_;
     } else {
       LOG(FATAL) << "Unknown uint32 field name: " << key;
     }
-    *out_len = static_cast<xgboost::bst_ulong>(vec->size());
+    *out_len = static_cast<boxhed_kernel::bst_ulong>(vec->size());
     *reinterpret_cast<unsigned const**>(out_dptr) = dmlc::BeginPtr(*vec);
   } else {
     LOG(FATAL) << "Unknown data type for getting meta info.";
   }
 }
 
 void MetaInfo::SetFeatureInfo(const char* key, const char **info, const bst_ulong size) {
@@ -930,15 +930,15 @@
   exec.Rethrow();
   omp_set_num_threads(nthread_original);
 
   return max_columns;
 }
 
 void SparsePage::PushCSC(const SparsePage &batch) {
-  std::vector<xgboost::Entry>& self_data = data.HostVector();
+  std::vector<boxhed_kernel::Entry>& self_data = data.HostVector();
   std::vector<bst_row_t>& self_offset = offset.HostVector();
 
   auto const& other_data = batch.data.ConstHostVector();
   auto const& other_offset = batch.offset.ConstHostVector();
 
   if (other_data.empty()) {
     return;
@@ -952,15 +952,15 @@
     self_offset = other_offset;
     return;
   }
 
   std::vector<bst_row_t> offset(other_offset.size());
   offset[0] = 0;
 
-  std::vector<xgboost::Entry> data(self_data.size() + other_data.size());
+  std::vector<boxhed_kernel::Entry> data(self_data.size() + other_data.size());
 
   // n_cols in original csr data matrix, here in csc is n_rows
   size_t const n_features = other_offset.size() - 1;
   size_t beg = 0;
   size_t ptr = 1;
   for (size_t i = 0; i < n_features; ++i) {
     size_t const self_beg = self_offset.at(i);
@@ -1004,8 +1004,8 @@
 SparsePage::Push(const data::FileAdapterBatch& batch, float missing, int nthread);
 
 namespace data {
 
 // List of files that will be force linked in static links.
 DMLC_REGISTRY_LINK_TAG(sparse_page_raw_format);
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/data.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/data.cu`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /*!
  * Copyright 2019 by XGBoost Contributors
  *
  * \file data.cu
  * \brief Handles setting metainfo from array interface.
  */
-#include "xgboost/data.h"
-#include "xgboost/logging.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/json.h"
 #include "array_interface.h"
 #include "../common/device_helpers.cuh"
 #include "device_adapter.cuh"
 #include "simple_dmatrix.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 void CopyInfoImpl(ArrayInterface column, HostDeviceVector<float>* out) {
   auto SetDeviceToPtr = [](void* ptr) {
     cudaPointerAttributes attr;
     dh::safe_cuda(cudaPointerGetAttributes(&attr, ptr));
     int32_t ptr_device = attr.device;
     dh::safe_cuda(cudaSetDevice(ptr_device));
@@ -125,8 +125,8 @@
 
 template DMatrix* DMatrix::Create<data::CudfAdapter>(
     data::CudfAdapter* adapter, float missing, int nthread,
     const std::string& cache_prefix, size_t page_size);
 template DMatrix* DMatrix::Create<data::CupyAdapter>(
     data::CupyAdapter* adapter, float missing, int nthread,
     const std::string& cache_prefix, size_t page_size);
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/device_adapter.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/device_adapter.cuh`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #include <memory>
 #include <string>
 #include "../common/device_helpers.cuh"
 #include "../common/math.h"
 #include "adapter.h"
 #include "array_interface.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 struct IsValidFunctor : public thrust::unary_function<Entry, bool> {
   explicit IsValidFunctor(float missing) : missing(missing) {}
 
   float missing;
   __device__ bool operator()(const data::COOTuple& e) const {
@@ -224,9 +224,9 @@
   size_t row_stride = dh::Reduce(
       thrust::cuda::par(alloc), thrust::device_pointer_cast(offset.data()),
       thrust::device_pointer_cast(offset.data()) + offset.size(), size_t(0),
       thrust::maximum<size_t>());
   return row_stride;
 }
 };  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_DATA_DEVICE_ADAPTER_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page.cc`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /*!
  * Copyright 2019 XGBoost contributors
  */
 #ifndef XGBOOST_USE_CUDA
 
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 
 // dummy implementation of EllpackPage in case CUDA is not used
-namespace xgboost {
+namespace boxhed_kernel {
 
 class EllpackPageImpl {};
 
 EllpackPage::EllpackPage() = default;
 
 EllpackPage::EllpackPage(DMatrix* dmat, const BatchParam& param) {
   LOG(FATAL) << "Internal Error: XGBoost is not compiled with CUDA but "
@@ -28,10 +28,10 @@
 }
 size_t EllpackPage::Size() const {
   LOG(FATAL) << "Internal Error: XGBoost is not compiled with CUDA but "
                 "EllpackPage is required";
   return 0;
 }
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_USE_CUDA
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page.cu`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 /*!
  * Copyright 2019-2020 XGBoost contributors
  */
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 #include <thrust/iterator/discard_iterator.h>
 #include <thrust/iterator/transform_output_iterator.h>
 #include "../common/categorical.h"
 #include "../common/hist_util.cuh"
 #include "../common/random.h"
 #include "./ellpack_page.cuh"
 #include "device_adapter.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 EllpackPage::EllpackPage() : impl_{new EllpackPageImpl()} {}
 
 EllpackPage::EllpackPage(DMatrix* dmat, const BatchParam& param)
     : impl_{new EllpackPageImpl(dmat, param)} {}
 
 EllpackPage::~EllpackPage() = default;
@@ -462,8 +462,8 @@
 EllpackDeviceAccessor EllpackPageImpl::GetDeviceAccessor(int device) const {
   gidx_buffer.SetDevice(device);
   return EllpackDeviceAccessor(
       device, cuts_, is_dense, row_stride, base_rowid, n_rows,
       common::CompressedIterator<uint32_t>(gidx_buffer.ConstDevicePointer(),
                                            NumSymbols()));
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page.cuh`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /*!
  * Copyright 2019 by XGBoost Contributors
  */
 
 #ifndef XGBOOST_DATA_ELLPACK_PAGE_H_
 #define XGBOOST_DATA_ELLPACK_PAGE_H_
 
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 
 #include "../common/compressed_iterator.h"
 #include "../common/device_helpers.cuh"
 #include "../common/hist_util.h"
 #include <thrust/binary_search.h>
 
-namespace xgboost {
+namespace boxhed_kernel {
 /** \brief Struct for accessing and manipulating an ellpack matrix on the
  * device. Does not own underlying memory and may be trivially copied into
  * kernels.*/
 struct EllpackDeviceAccessor {
   /*! \brief Whether or not if the matrix is dense. */
   bool is_dense;
   /*! \brief Row length for ELLPack, equal to number of features. */
@@ -218,10 +218,10 @@
     for (auto i = 1ull; i < row_offset.size(); i++) {
       row_stride = std::max(
         row_stride, static_cast<size_t>(row_offset[i] - row_offset[i - 1]));
     }
   }
   return row_stride;
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_DATA_ELLPACK_PAGE_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page_raw_format.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page_raw_format.cu`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 /*!
  * Copyright 2019 XGBoost contributors
  */
 
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 #include <dmlc/registry.h>
 
 #include "./ellpack_page.cuh"
 #include "./sparse_page_writer.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 DMLC_REGISTRY_FILE_TAG(ellpack_page_raw_format);
 
 class EllpackPageRawFormat : public SparsePageFormat<EllpackPage> {
  public:
   bool Read(EllpackPage* page, dmlc::SeekStream* fi) override {
@@ -52,8 +52,8 @@
 XGBOOST_REGISTER_ELLPACK_PAGE_FORMAT(raw)
     .describe("Raw ELLPACK binary data format.")
     .set_body([]() {
       return new EllpackPageRawFormat();
     });
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page_source.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page_source.cc`

 * *Files 24% similar despite different names*

```diff
@@ -2,23 +2,23 @@
  * Copyright 2019 XGBoost contributors
  */
 #ifndef XGBOOST_USE_CUDA
 #include <dmlc/base.h>
 #if DMLC_ENABLE_STD_THREAD
 
 #include "ellpack_page_source.h"
-#include <xgboost/data.h>
-namespace xgboost {
+#include <boxhed_kernel/data.h>
+namespace boxhed_kernel {
 namespace data {
 
 EllpackPageSource::EllpackPageSource(DMatrix* dmat,
                                      const std::string& cache_info,
                                      const BatchParam& param) noexcept(false) {
   LOG(FATAL)
       << "Internal Error: "
          "XGBoost is not compiled with CUDA but EllpackPageSource is required";
 }
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // DMLC_ENABLE_STD_THREAD
 #endif  // XGBOOST_USE_CUDA
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page_source.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page_source.cu`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 #include "../common/hist_util.cuh"
 
 #include "ellpack_page.cuh"
 #include "ellpack_page_source.h"
 #include "sparse_page_source.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 // Build the quantile sketch across the whole input data, then use the histogram cuts to compress
 // each CSR page, and write the accumulated ELLPACK pages to disk.
 EllpackPageSource::EllpackPageSource(DMatrix* dmat,
                                      const std::string& cache_info,
                                      const BatchParam& param) noexcept(false) {
@@ -82,8 +82,8 @@
     *impl = EllpackPageImpl(device, cuts, temp_host_page, dmat->IsDense(),
                             row_stride, ft);
     writer.PushWrite(std::move(page));
   }
 }
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/ellpack_page_source.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/ellpack_page_source.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 /*!
  * Copyright 2019 by XGBoost Contributors
  */
 
 #ifndef XGBOOST_DATA_ELLPACK_PAGE_SOURCE_H_
 #define XGBOOST_DATA_ELLPACK_PAGE_SOURCE_H_
 
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 #include <memory>
 #include <string>
 
 #include "../common/timer.h"
 #include "../common/hist_util.h"
 #include "sparse_page_source.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 /*!
  * \brief External memory data source for ELLPACK format.
  *
  */
 class EllpackPageSource {
@@ -56,10 +56,10 @@
   size_t page_size_{DMatrix::kPageSize};
   common::Monitor monitor_;
   std::unique_ptr<ExternalMemoryPrefetcher<EllpackPage>> external_prefetcher_;
   CacheInfo cache_info_;
 };
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_DATA_ELLPACK_PAGE_SOURCE_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/iterative_device_dmatrix.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/iterative_device_dmatrix.cu`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #include "simple_batch_iterator.h"
 #include "iterative_device_dmatrix.h"
 #include "sparse_page_source.h"
 #include "ellpack_page.cuh"
 #include "proxy_dmatrix.h"
 #include "device_adapter.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 template <typename Fn>
 decltype(auto) Dispatch(DMatrixProxy const* proxy, Fn fn) {
   if (proxy->Adapter().type() == typeid(std::shared_ptr<CupyAdapter>)) {
     auto value = dmlc::get<std::shared_ptr<CupyAdapter>>(
         proxy->Adapter())->Value();
@@ -178,8 +178,8 @@
 BatchSet<EllpackPage> IterativeDeviceDMatrix::GetEllpackBatches(const BatchParam& param) {
   CHECK(page_);
   auto begin_iter =
       BatchIterator<EllpackPage>(new SimpleBatchIteratorImpl<EllpackPage>(page_.get()));
   return BatchSet<EllpackPage>(begin_iter);
 }
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/iterative_device_dmatrix.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/iterative_device_dmatrix.h`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 #define XGBOOST_DATA_ITERATIVE_DEVICE_DMATRIX_H_
 
 #include <vector>
 #include <string>
 #include <utility>
 #include <memory>
 
-#include "xgboost/base.h"
-#include "xgboost/data.h"
-#include "xgboost/c_api.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/c_api.h"
 #include "proxy_dmatrix.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 class IterativeDeviceDMatrix : public DMatrix {
   MetaInfo info_;
   BatchParam batch_param_;
   std::shared_ptr<EllpackPage> page_;
 
@@ -67,10 +67,10 @@
     return info_;
   }
   MetaInfo const& Info() const override {
     return info_;
   }
 };
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_DATA_ITERATIVE_DEVICE_DMATRIX_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/proxy_dmatrix.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/proxy_dmatrix.cu`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*!
  * Copyright 2020 XGBoost contributors
  */
 #include "proxy_dmatrix.h"
 #include "device_adapter.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 void DMatrixProxy::FromCudaColumnar(std::string interface_str) {
   std::shared_ptr<data::CudfAdapter> adapter {new data::CudfAdapter(interface_str)};
   auto const& value = adapter->Value();
   this->batch_ = adapter;
   device_ = adapter->DeviceIdx();
@@ -21,8 +21,8 @@
   this->batch_ = adapter;
   device_ = adapter->DeviceIdx();
   this->Info().num_col_ = adapter->NumColumns();
   this->Info().num_row_ = adapter->NumRows();
 }
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/proxy_dmatrix.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/proxy_dmatrix.h`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 #include <dmlc/any.h>
 
 #include <memory>
 #include <string>
 #include <utility>
 
-#include "xgboost/data.h"
-#include "xgboost/generic_parameters.h"
-#include "xgboost/c_api.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/generic_parameters.h"
+#include "boxhed_kernel/c_api.h"
 #include "adapter.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 /*
  * \brief A proxy to external iterator.
  */
 template <typename ResetFn, typename NextFn>
 class DataIterProxy {
   DataIterHandle iter_;
@@ -41,15 +41,15 @@
 
 /*
  * \brief A proxy of DMatrix used by external iterator.
  */
 class DMatrixProxy : public DMatrix {
   MetaInfo info_;
   dmlc::any batch_;
-  int32_t device_ { xgboost::GenericParameter::kCpuId };
+  int32_t device_ { boxhed_kernel::GenericParameter::kCpuId };
 
 #if defined(XGBOOST_USE_CUDA)
   void FromCudaColumnar(std::string interface_str);
   void FromCudaArray(std::string interface_str);
 #endif  // defined(XGBOOST_USE_CUDA)
 
  public:
@@ -99,9 +99,9 @@
   }
 
   dmlc::any Adapter() const {
     return batch_;
   }
 };
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_DATA_PROXY_DMATRIX_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/simple_dmatrix.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/simple_dmatrix.cc`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,24 @@
  * \author Tianqi Chen
  */
 #include <vector>
 #include <limits>
 #include <type_traits>
 #include <algorithm>
 
-#include "xgboost/data.h"
-#include "xgboost/c_api.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/c_api.h"
 
 #include "simple_dmatrix.h"
 #include "./simple_batch_iterator.h"
 #include "../common/random.h"
 #include "../common/threading_utils.h"
 #include "adapter.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 MetaInfo& SimpleDMatrix::Info() { return info_; }
 
 const MetaInfo& SimpleDMatrix::Info() const { return info_; }
 
 DMatrix* SimpleDMatrix::Slice(common::Span<int32_t const> ridxs) {
   auto out = new SimpleDMatrix;
@@ -217,8 +217,8 @@
 template SimpleDMatrix::SimpleDMatrix(FileAdapter* adapter, float missing,
                                      int nthread);
 template SimpleDMatrix::SimpleDMatrix(
     IteratorAdapter<DataIterHandle, XGBCallbackDataIterNext, XGBoostBatchCSR>
         *adapter,
     float missing, int nthread);
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/simple_dmatrix.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/simple_dmatrix.cu`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 /*!
  * Copyright 2019 by Contributors
  * \file simple_dmatrix.cu
  */
 #include <thrust/copy.h>
 #include <thrust/execution_policy.h>
 #include <thrust/sort.h>
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 #include "../common/random.h"
 #include "./simple_dmatrix.h"
 #include "device_adapter.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 
 template <typename AdapterBatchT>
 void CountRowOffsets(const AdapterBatchT& batch, common::Span<bst_row_t> offset,
                      int device_idx, float missing) {
   IsValidFunctor is_valid(missing);
@@ -100,8 +100,8 @@
 }
 
 template SimpleDMatrix::SimpleDMatrix(CudfAdapter* adapter, float missing,
                                       int nthread);
 template SimpleDMatrix::SimpleDMatrix(CupyAdapter* adapter, float missing,
                                       int nthread);
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/simple_dmatrix.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/simple_dmatrix.h`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
  * \file simple_dmatrix.h
  * \brief In-memory version of DMatrix.
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_DATA_SIMPLE_DMATRIX_H_
 #define XGBOOST_DATA_SIMPLE_DMATRIX_H_
 
-#include <xgboost/base.h>
-#include <xgboost/data.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/data.h>
 
 #include <memory>
 #include <string>
 
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 // Used for single batch data.
 class SimpleDMatrix : public DMatrix {
  public:
   SimpleDMatrix() = default;
   template <typename AdapterT>
   explicit SimpleDMatrix(AdapterT* adapter, float missing, int nthread);
@@ -55,9 +55,9 @@
     return static_cast<bool>(ellpack_page_);
   }
   bool SparsePageExists() const override {
     return true;
   }
 };
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_DATA_SIMPLE_DMATRIX_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_dmatrix.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_dmatrix.cc`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #include <dmlc/timer.h>
 
 #if DMLC_ENABLE_STD_THREAD
 #include "./sparse_page_dmatrix.h"
 
 #include "./simple_batch_iterator.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 MetaInfo& SparsePageDMatrix::Info() {
   return row_source_->info;
 }
 
 const MetaInfo& SparsePageDMatrix::Info() const {
@@ -51,9 +51,9 @@
     ellpack_source_.reset(new EllpackPageSource(this, cache_info_, param));
     batch_param_ = param;
   }
   return ellpack_source_->GetBatchSet();
 }
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // DMLC_ENABLE_STD_THREAD
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_dmatrix.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_dmatrix.h`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,25 @@
  * \file sparse_page_dmatrix.h
  * \brief External-memory version of DMatrix.
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_DATA_SPARSE_PAGE_DMATRIX_H_
 #define XGBOOST_DATA_SPARSE_PAGE_DMATRIX_H_
 
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 #include <algorithm>
 #include <memory>
 #include <string>
 #include <utility>
 #include <vector>
 
 #include "ellpack_page_source.h"
 #include "sparse_page_source.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 // Used for external memory.
 class SparsePageDMatrix : public DMatrix {
  public:
   template <typename AdapterT>
   explicit SparsePageDMatrix(AdapterT* adapter, float missing, int nthread,
                              const std::string& cache_prefix,
@@ -64,9 +64,9 @@
     return static_cast<bool>(ellpack_source_);
   }
   bool SparsePageExists() const override {
     return static_cast<bool>(row_source_);
   }
 };
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_DATA_SPARSE_PAGE_DMATRIX_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_raw_format.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_raw_format.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 /*!
  * Copyright (c) 2015 by Contributors
  * \file sparse_page_raw_format.cc
  *  Raw binary format of sparse page.
  */
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 #include <dmlc/registry.h>
 #include "./sparse_page_writer.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 DMLC_REGISTRY_FILE_TAG(sparse_page_raw_format);
 
 template<typename T>
 class SparsePageRawFormat : public SparsePageFormat<T> {
  public:
@@ -111,8 +111,8 @@
 XGBOOST_REGISTER_SORTED_CSC_PAGE_FORMAT(raw)
 .describe("Raw binary data format.")
 .set_body([]() {
     return new SparsePageRawFormat<SortedCSCPage>();
   });
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_source.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_source.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 /*!
  *  Copyright (c) 2020 by XGBoost Contributors
  */
 #include "sparse_page_source.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 void DataPool::Slice(std::shared_ptr<SparsePage> out, size_t offset,
                      size_t n_rows, size_t entry_offset) const {
   auto const &in_offset = pool_.offset.HostVector();
   auto const &in_data = pool_.data.HostVector();
   auto &h_offset = out->offset.HostVector();
   CHECK_LE(offset + n_rows + 1, in_offset.size());
@@ -70,8 +70,8 @@
     page->Clear();
     this->writer_->PushWrite(std::move(page));
   }
 
   return inferred_num_rows_;
 }
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_source.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_source.h`

 * *Files 2% similar despite different names*

```diff
@@ -47,44 +47,44 @@
 #include <memory>
 #include <string>
 #include <utility>
 #include <vector>
 #include <fstream>
 
 #include "rabit/rabit.h"
-#include "xgboost/base.h"
-#include "xgboost/data.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
 
 #include "adapter.h"
 #include "sparse_page_writer.h"
 #include "../common/common.h"
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 
 namespace detail {
 
 // Split a cache info string with delimiter ':'
 // If cache info string contains drive letter (e.g. C:), exclude it before splitting
 inline std::vector<std::string>
 GetCacheShards(const std::string& cache_info) {
 #if (defined _WIN32) || (defined __CYGWIN__)
   if (cache_info.length() >= 2
       && std::isalpha(cache_info[0], std::locale::classic())
       && cache_info[1] == ':') {
     std::vector<std::string> cache_shards
-      = xgboost::common::Split(cache_info.substr(2), ':');
+      = boxhed_kernel::common::Split(cache_info.substr(2), ':');
     cache_shards[0] = cache_info.substr(0, 2) + cache_shards[0];
     return cache_shards;
   }
 #endif  // (defined _WIN32) || (defined __CYGWIN__)
-  return xgboost::common::Split(cache_info, ':');
+  return boxhed_kernel::common::Split(cache_info, ':');
 }
 
 }  // namespace detail
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 template<typename S, typename T>
 class SparseBatchIteratorImpl : public BatchIteratorImpl<T> {
  public:
   explicit SparseBatchIteratorImpl(S* source) : source_(source) {
     CHECK(source_ != nullptr);
@@ -556,9 +556,9 @@
 
  private:
   std::unique_ptr<ExternalMemoryPrefetcher<SortedCSCPage>> external_prefetcher_;
   CacheInfo cache_info_;
 };
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_DATA_SPARSE_PAGE_SOURCE_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/data/sparse_page_writer.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/data/sparse_page_writer.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
  * Copyright (c) 2014-2019 by Contributors
  * \file sparse_page_writer.h
  * \author Tianqi Chen
  */
 #ifndef XGBOOST_DATA_SPARSE_PAGE_WRITER_H_
 #define XGBOOST_DATA_SPARSE_PAGE_WRITER_H_
 
-#include <xgboost/data.h>
+#include <boxhed_kernel/data.h>
 #include <dmlc/io.h>
 #include <vector>
 #include <algorithm>
 #include <cstring>
 #include <string>
 #include <utility>
 #include <memory>
 #include <functional>
 
 #if DMLC_ENABLE_STD_THREAD
 #include <dmlc/concurrency.h>
 #include <thread>
 #endif  // DMLC_ENABLE_STD_THREAD
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace data {
 
 template<typename T>
 struct SparsePageFormatReg;
 
 /*!
  * \brief Format specification of SparsePage.
@@ -205,9 +205,9 @@
   DMLC_REGISTRY_REGISTER(SparsePageFormatReg<SortedCSCPage>, SortedCSCPageFmt, Name)
 
 #define EllpackPageFmt SparsePageFormat<EllpackPage>
 #define XGBOOST_REGISTER_ELLPACK_PAGE_FORMAT(Name)                       \
   DMLC_REGISTRY_REGISTER(SparsePageFormatReg<EllpackPage>, EllpackPageFm, Name)
 
 }  // namespace data
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_DATA_SPARSE_PAGE_WRITER_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gblinear.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gblinear.cc`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 #include <dmlc/parameter.h>
 
 #include <vector>
 #include <string>
 #include <sstream>
 #include <algorithm>
 
-#include "xgboost/gbm.h"
-#include "xgboost/json.h"
-#include "xgboost/predictor.h"
-#include "xgboost/linear_updater.h"
-#include "xgboost/logging.h"
-#include "xgboost/learner.h"
+#include "boxhed_kernel/gbm.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/predictor.h"
+#include "boxhed_kernel/linear_updater.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/learner.h"
 
 #include "gblinear_model.h"
 #include "../common/timer.h"
 #include "../common/common.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace gbm {
 
 DMLC_REGISTRY_FILE_TAG(gblinear);
 
 // training parameters
 struct GBLinearTrainParam : public XGBoostParameter<GBLinearTrainParam> {
   std::string updater;
@@ -307,8 +307,8 @@
 
 XGBOOST_REGISTER_GBM(GBLinear, "gblinear")
     .describe("Linear booster, implement generalized linear model.")
     .set_body([](LearnerModelParam const* booster_config) {
       return new GBLinear(booster_config);
     });
 }  // namespace gbm
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gblinear_model.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gblinear_model.cc`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /*!
  * Copyright 2019 by Contributors
  */
 #include <utility>
 #include <limits>
-#include "xgboost/json.h"
+#include "boxhed_kernel/json.h"
 #include "gblinear_model.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace gbm {
 
 void GBLinearModel::SaveModel(Json* p_out) const {
   using WeightType = std::remove_reference<decltype(std::declval<decltype(weight)>().back())>::type;
   using JsonFloat = Number::Float;
   static_assert(std::is_same<WeightType, JsonFloat>::value,
                 "Weight type should be of the same type with JSON float");
@@ -31,8 +31,8 @@
   for (size_t i = 0; i < n_weights; ++i) {
     weight[i] = get<Number const>(j_weights[i]);
   }
 }
 
 DMLC_REGISTER_PARAMETER(DeprecatedGBLinearModelParam);
 }  // namespace gbm
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gblinear_model.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gblinear_model.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*!
  * Copyright 2018-2019 by Contributors
  */
 #pragma once
 #include <dmlc/io.h>
 #include <dmlc/parameter.h>
-#include <xgboost/learner.h>
+#include <boxhed_kernel/learner.h>
 
 #include <vector>
 #include <string>
 #include <cstring>
 
-#include "xgboost/base.h"
-#include "xgboost/feature_map.h"
-#include "xgboost/model.h"
-#include "xgboost/json.h"
-#include "xgboost/parameter.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/feature_map.h"
+#include "boxhed_kernel/model.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/parameter.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 class Json;
 namespace gbm {
 // Deprecated in 1.0.0. model parameter.  Only staying here for compatible binary model IO.
 struct DeprecatedGBLinearModelParam : public dmlc::Parameter<DeprecatedGBLinearModelParam> {
   // number of feature dimension
   uint32_t deprecated_num_feature;
   // deprecated. use learner_model_param_->num_output_group.
@@ -136,8 +136,8 @@
     std::vector<std::string> v;
     v.push_back(fo.str());
     return v;
   }
 };
 
 }  // namespace gbm
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbm.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbm.cc`

 * *Files 15% similar despite different names*

```diff
@@ -4,37 +4,37 @@
  * \brief Registry of gradient boosters.
  */
 #include <dmlc/registry.h>
 #include <string>
 #include <vector>
 #include <memory>
 
-#include "xgboost/gbm.h"
-#include "xgboost/learner.h"
-#include "xgboost/generic_parameters.h"
+#include "boxhed_kernel/gbm.h"
+#include "boxhed_kernel/learner.h"
+#include "boxhed_kernel/generic_parameters.h"
 
 namespace dmlc {
-DMLC_REGISTRY_ENABLE(::xgboost::GradientBoosterReg);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::GradientBoosterReg);
 }  // namespace dmlc
 
-namespace xgboost {
+namespace boxhed_kernel {
 GradientBooster* GradientBooster::Create(
     const std::string& name,
     GenericParameter const* generic_param,
     LearnerModelParam const* learner_model_param) {
-  auto *e = ::dmlc::Registry< ::xgboost::GradientBoosterReg>::Get()->Find(name);
+  auto *e = ::dmlc::Registry< ::boxhed_kernel::GradientBoosterReg>::Get()->Find(name);
   if (e == nullptr) {
     LOG(FATAL) << "Unknown gbm type " << name;
   }
   auto p_bst =  (e->body)(learner_model_param);
   p_bst->generic_param_ = generic_param;
   return p_bst;
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace gbm {
 // List of files that will be force linked in static links.
 DMLC_REGISTRY_LINK_TAG(gblinear);
 DMLC_REGISTRY_LINK_TAG(gbtree);
 }  // namespace gbm
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbtree.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbtree.cc`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 #include <vector>
 #include <memory>
 #include <utility>
 #include <string>
 #include <limits>
 #include <algorithm>
 
-#include "xgboost/data.h"
-#include "xgboost/gbm.h"
-#include "xgboost/logging.h"
-#include "xgboost/json.h"
-#include "xgboost/predictor.h"
-#include "xgboost/tree_updater.h"
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/gbm.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/predictor.h"
+#include "boxhed_kernel/tree_updater.h"
+#include "boxhed_kernel/host_device_vector.h"
 
 #include "gbtree.h"
 #include "gbtree_model.h"
 #include "../common/common.h"
 #include "../common/random.h"
 #include "../common/timer.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace gbm {
 
 DMLC_REGISTRY_FILE_TAG(gbtree);
 
 void GBTree::Configure(const Args& cfg) {
   this->cfg_ = cfg;
   std::string updater_seq = tparam_.updater_seq;
@@ -334,15 +334,15 @@
 void GBTree::LoadConfig(Json const& in) {
   CHECK_EQ(get<String>(in["name"]), "gbtree");
   FromJson(in["gbtree_train_param"], &tparam_);
   // Process type cannot be kUpdate from loaded model
   // This would cause all trees to be pushed to trees_to_update
   // e.g. updating a model, then saving and loading it would result in an empty model
   tparam_.process_type = TreeProcessType::kDefault;
-  int32_t const n_gpus = xgboost::common::AllVisibleGPUs();
+  int32_t const n_gpus = boxhed_kernel::common::AllVisibleGPUs();
   if (n_gpus == 0 && tparam_.predictor == PredictorType::kGPUPredictor) {
     LOG(WARNING)
         << "Loading from a raw memory buffer on CPU only machine.  "
            "Changing predictor to auto.";
     tparam_.UpdateAllowUnknown(Args{{"predictor", "auto"}});
   }
   if (n_gpus == 0 && tparam_.tree_method == TreeMethod::kGPUHist) {
@@ -870,8 +870,8 @@
 XGBOOST_REGISTER_GBM(Dart, "dart")
 .describe("Tree booster, dart.")
 .set_body([](LearnerModelParam const* booster_config) {
     GBTree* p = new Dart(booster_config);
     return p;
   });
 }  // namespace gbm
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbtree.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbtree.h`

 * *Files 6% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 #include <vector>
 #include <map>
 #include <memory>
 #include <utility>
 #include <string>
 #include <unordered_map>
 
-#include "xgboost/base.h"
-#include "xgboost/data.h"
-#include "xgboost/logging.h"
-#include "xgboost/gbm.h"
-#include "xgboost/predictor.h"
-#include "xgboost/tree_updater.h"
-#include "xgboost/parameter.h"
-#include "xgboost/json.h"
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/gbm.h"
+#include "boxhed_kernel/predictor.h"
+#include "boxhed_kernel/tree_updater.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/host_device_vector.h"
 
 #include "gbtree_model.h"
 #include "../common/common.h"
 #include "../common/timer.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 enum class TreeMethod : int {
   kAuto = 0, kApprox = 1, kExact = 2, kHist = 3,
   kGPUHist = 5
 };
 
 // boosting process types
 enum class TreeProcessType : int {
@@ -44,21 +44,21 @@
 
 enum class PredictorType : int {
   kAuto = 0,
   kCPUPredictor,
   kGPUPredictor,
   kOneAPIPredictor
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
-DECLARE_FIELD_ENUM_CLASS(xgboost::TreeMethod);
-DECLARE_FIELD_ENUM_CLASS(xgboost::TreeProcessType);
-DECLARE_FIELD_ENUM_CLASS(xgboost::PredictorType);
+DECLARE_FIELD_ENUM_CLASS(boxhed_kernel::TreeMethod);
+DECLARE_FIELD_ENUM_CLASS(boxhed_kernel::TreeProcessType);
+DECLARE_FIELD_ENUM_CLASS(boxhed_kernel::PredictorType);
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace gbm {
 
 /*! \brief training parameters */
 struct GBTreeTrainParam : public XGBoostParameter<GBTreeTrainParam> {
   /*!
    * \brief number of parallel trees constructed each iteration
    *  use this option to support boosted random forest
@@ -344,10 +344,10 @@
 #if defined(XGBOOST_USE_ONEAPI)
   std::unique_ptr<Predictor> oneapi_predictor_;
 #endif  // defined(XGBOOST_USE_ONEAPI)
   common::Monitor monitor_;
 };
 
 }  // namespace gbm
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_GBM_GBTREE_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbtree_model.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbtree_model.cc`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 /*!
  * Copyright 2019-2020 by Contributors
  */
 #include <utility>
 
-#include "xgboost/json.h"
-#include "xgboost/logging.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/logging.h"
 #include "gbtree_model.h"
 #include "gbtree.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace gbm {
 void GBTreeModel::Save(dmlc::Stream* fo) const {
   CHECK_EQ(param.num_trees, static_cast<int32_t>(trees.size()));
 
   if (DMLC_IO_NO_ENDIAN_SWAP) {
     fo->Write(&param, sizeof(param));
   } else {
@@ -105,8 +105,8 @@
   auto const& tree_info_json = get<Array const>(in["tree_info"]);
   for (int32_t i = 0; i < param.num_trees; ++i) {
     tree_info[i] = get<Integer const>(tree_info_json[i]);
   }
 }
 
 }  // namespace gbm
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/gbm/gbtree_model.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/gbm/gbtree_model.h`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,25 @@
  * \file gbtree_model.h
  */
 #ifndef XGBOOST_GBM_GBTREE_MODEL_H_
 #define XGBOOST_GBM_GBTREE_MODEL_H_
 
 #include <dmlc/parameter.h>
 #include <dmlc/io.h>
-#include <xgboost/model.h>
-#include <xgboost/tree_model.h>
-#include <xgboost/parameter.h>
-#include <xgboost/learner.h>
+#include <boxhed_kernel/model.h>
+#include <boxhed_kernel/tree_model.h>
+#include <boxhed_kernel/parameter.h>
+#include <boxhed_kernel/learner.h>
 
 #include <memory>
 #include <utility>
 #include <string>
 #include <vector>
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 class Json;
 
 namespace gbm {
 
 /*! \brief model parameters */
 struct GBTreeModelParam : public dmlc::Parameter<GBTreeModelParam> {
@@ -132,10 +132,10 @@
   std::vector<std::unique_ptr<RegTree> > trees;
   /*! \brief for the update process, a place to keep the initial trees */
   std::vector<std::unique_ptr<RegTree> > trees_to_update;
   /*! \brief some information indicator of the tree, reserved */
   std::vector<int> tree_info;
 };
 }  // namespace gbm
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_GBM_GBTREE_MODEL_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/learner.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/learner.cc`

 * *Files 3% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 #include <sstream>
 #include <string>
 #include <stack>
 #include <utility>
 #include <vector>
 
 #include "dmlc/any.h"
-#include "xgboost/base.h"
-#include "xgboost/data.h"
-#include "xgboost/model.h"
-#include "xgboost/predictor.h"
-#include "xgboost/feature_map.h"
-#include "xgboost/gbm.h"
-#include "xgboost/generic_parameters.h"
-#include "xgboost/host_device_vector.h"
-#include "xgboost/json.h"
-#include "xgboost/learner.h"
-#include "xgboost/logging.h"
-#include "xgboost/metric.h"
-#include "xgboost/objective.h"
-#include "xgboost/parameter.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/model.h"
+#include "boxhed_kernel/predictor.h"
+#include "boxhed_kernel/feature_map.h"
+#include "boxhed_kernel/gbm.h"
+#include "boxhed_kernel/generic_parameters.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/learner.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/metric.h"
+#include "boxhed_kernel/objective.h"
+#include "boxhed_kernel/parameter.h"
 
 #include "common/common.h"
 #include "common/io.h"
 #include "common/observer.h"
 #include "common/random.h"
 #include "common/timer.h"
 #include "common/charconv.h"
@@ -46,24 +46,24 @@
 #include "common/threading_utils.h"
 
 namespace {
 
 const char* kMaxDeltaStepDefaultValue = "0.7";
 }  // anonymous namespace
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 enum class DataSplitMode : int {
   kAuto = 0, kCol = 1, kRow = 2
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
-DECLARE_FIELD_ENUM_CLASS(xgboost::DataSplitMode);
+DECLARE_FIELD_ENUM_CLASS(boxhed_kernel::DataSplitMode);
 
-namespace xgboost {
+namespace boxhed_kernel {
 // implementation of base learner.
 bool Learner::AllowLazyCheckPoint() const {
   return gbm_->AllowLazyCheckPoint();
 }
 
 Learner::~Learner() = default;
 
@@ -919,15 +919,15 @@
           << R"doc(
 
   If you are loading a serialized model (like pickle in Python) generated by older
   XGBoost, please export the model by calling `Booster.save_model` from that version
   first, then load it back in current version.  There's a simple script for helping
   the process. See:
 
-    https://xgboost.readthedocs.io/en/latest/tutorials/saving_model.html
+    https://boxhed_kernel.readthedocs.io/en/latest/tutorials/saving_model.html
 
   for reference to the script, and more details about differences between saving model and
   serializing.
 
 )doc";
       int64_t sz {-1};
       CHECK_EQ(fp.Read(&sz, sizeof(sz)), sizeof(sz));
@@ -1199,8 +1199,8 @@
 
 constexpr int32_t LearnerImpl::kRandSeedMagic;
 
 Learner* Learner::Create(
     const std::vector<std::shared_ptr<DMatrix> >& cache_data) {
   return new LearnerImpl(cache_data);
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/linear/coordinate_common.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/linear/coordinate_common.h`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 #pragma once
 #include <algorithm>
 #include <string>
 #include <utility>
 #include <vector>
 #include <limits>
 
-#include "xgboost/data.h"
-#include "xgboost/parameter.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/parameter.h"
 #include "./param.h"
 #include "../gbm/gblinear_model.h"
 #include "../common/random.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace linear {
 
 struct CoordinateParam : public XGBoostParameter<CoordinateParam> {
   int top_k;
   DMLC_DECLARE_PARAMETER(CoordinateParam) {
     DMLC_DECLARE_FIELD(top_k)
         .set_lower_bound(0)
@@ -473,8 +473,8 @@
     default:
       LOG(FATAL) << "unknown coordinate selector: " << choice;
   }
   return nullptr;
 }
 
 }  // namespace linear
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/linear/param.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/linear/param.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 /*!
  * Copyright 2018 by Contributors
  * \file param.h
  * \brief training parameters.
  */
 #ifndef XGBOOST_LINEAR_PARAM_H_
 #define XGBOOST_LINEAR_PARAM_H_
-#include "xgboost/parameter.h"
+#include "boxhed_kernel/parameter.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace linear {
 /**
  * \brief A set of available FeatureSelector's
  */
 enum FeatureSelectorEnum {
   kCyclic = 0,
   kShuffle,
@@ -62,10 +62,10 @@
   }
   // denormalizated regularization penalties
   float reg_lambda_denorm;
   float reg_alpha_denorm;
 };
 
 }  // namespace linear
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_LINEAR_PARAM_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/linear/updater_coordinate.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/linear/updater_coordinate.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /*!
  * Copyright 2018 by Contributors
  * \author Rory Mitchell
  */
 
-#include <xgboost/linear_updater.h>
+#include <boxhed_kernel/linear_updater.h>
 #include "./param.h"
 #include "../common/timer.h"
 #include "coordinate_common.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/json.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace linear {
 
 DMLC_REGISTER_PARAMETER(CoordinateParam);
 DMLC_REGISTRY_FILE_TAG(updater_coordinate);
 
 // training parameter
 /**
@@ -98,8 +98,8 @@
   common::Monitor monitor_;
 };
 
 XGBOOST_REGISTER_LINEAR_UPDATER(CoordinateUpdater, "coord_descent")
     .describe("Update linear model according to coordinate descent algorithm.")
     .set_body([]() { return new CoordinateUpdater(); });
 }  // namespace linear
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/linear/updater_gpu_coordinate.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/linear/updater_gpu_coordinate.cu`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 /*!
  * Copyright 2018-2019 by Contributors
  * \author Rory Mitchell
  */
 
 #include <thrust/execution_policy.h>
 #include <thrust/inner_product.h>
-#include <xgboost/data.h>
-#include <xgboost/linear_updater.h>
-#include "xgboost/span.h"
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/linear_updater.h>
+#include "boxhed_kernel/span.h"
 
 #include "coordinate_common.h"
 #include "../common/common.h"
 #include "../common/device_helpers.cuh"
 #include "../common/timer.h"
 #include "./param.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace linear {
 
 DMLC_REGISTRY_FILE_TAG(updater_gpu_coordinate);
 
 /**
  * \class GPUCoordinateUpdater
  *
@@ -74,18 +74,18 @@
     for (size_t fidx = 0; fidx < batch.Size(); fidx++) {
       common::Span<Entry const> col = batch[fidx];
       auto cmp = [](Entry e1, Entry e2) {
         return e1.index < e2.index;
       };
       auto column_begin =
           std::lower_bound(col.cbegin(), col.cend(),
-                           xgboost::Entry(0, 0.0f), cmp);
+                           boxhed_kernel::Entry(0, 0.0f), cmp);
       auto column_end =
           std::lower_bound(col.cbegin(), col.cend(),
-                           xgboost::Entry(num_row_, 0.0f), cmp);
+                           boxhed_kernel::Entry(num_row_, 0.0f), cmp);
       column_segments.emplace_back(
           std::make_pair(column_begin - col.cbegin(), column_end - col.cbegin()));
       row_ptr_.push_back(row_ptr_.back() + (column_end - column_begin));
     }
     data_.resize(row_ptr_.back());
     gpair_.resize(num_row_ * model_param.num_output_group);
     for (size_t fidx = 0; fidx < batch.Size(); fidx++) {
@@ -197,15 +197,15 @@
       g += GradientPair(g.GetHess() * dbias, 0);
     });
   }
 
   // This needs to be public because of the __device__ lambda.
   GradientPair GetGradient(int group_idx, int num_group, int fidx) {
     dh::safe_cuda(cudaSetDevice(learner_param_->gpu_id));
-    common::Span<xgboost::Entry> d_col = dh::ToSpan(data_).subspan(row_ptr_[fidx]);
+    common::Span<boxhed_kernel::Entry> d_col = dh::ToSpan(data_).subspan(row_ptr_[fidx]);
     size_t col_size = row_ptr_[fidx + 1] - row_ptr_[fidx];
     common::Span<GradientPair> d_gpair = dh::ToSpan(gpair_);
     auto counting = thrust::make_counting_iterator(0ull);
     auto f = [=] __device__(size_t idx) {
       auto entry = d_col[idx];
       auto g = d_gpair[entry.index * num_group + group_idx];
       return GradientPair(g.GetGrad() * entry.fvalue,
@@ -243,19 +243,19 @@
   // training parameter
   LinearTrainParam tparam_;
   CoordinateParam coord_param_;
   std::unique_ptr<FeatureSelector> selector_;
   common::Monitor monitor_;
 
   std::vector<size_t> row_ptr_;
-  dh::device_vector<xgboost::Entry> data_;
+  dh::device_vector<boxhed_kernel::Entry> data_;
   dh::caching_device_vector<GradientPair> gpair_;
   size_t num_row_;
 };
 
 XGBOOST_REGISTER_LINEAR_UPDATER(GPUCoordinateUpdater, "gpu_coord_descent")
     .describe(
         "Update linear model according to coordinate descent algorithm. GPU "
         "accelerated.")
     .set_body([]() { return new GPUCoordinateUpdater(); });
 }  // namespace linear
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/linear/updater_shotgun.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/linear/updater_shotgun.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /*!
  * Copyright 2018 by Contributors
  * \author Tianqi Chen, Rory Mitchell
  */
 
-#include <xgboost/linear_updater.h>
+#include <boxhed_kernel/linear_updater.h>
 #include "coordinate_common.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace linear {
 
 DMLC_REGISTRY_FILE_TAG(updater_shotgun);
 
 class ShotgunUpdater : public LinearUpdater {
  public:
   // set training parameter
@@ -97,8 +97,8 @@
 
 XGBOOST_REGISTER_LINEAR_UPDATER(ShotgunUpdater, "shotgun")
     .describe(
         "Update linear model according to shotgun coordinate descent "
         "algorithm.")
     .set_body([]() { return new ShotgunUpdater(); });
 }  // namespace linear
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/logging.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/logging.cc`

 * *Files 4% similar despite different names*

```diff
@@ -5,44 +5,44 @@
  * \author Tianqi Chen
  */
 #include <rabit/rabit.h>
 
 #include <iostream>
 #include <map>
 
-#include "xgboost/parameter.h"
-#include "xgboost/logging.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/logging.h"
 
 #if !defined(XGBOOST_STRICT_R_MODE) || XGBOOST_STRICT_R_MODE == 0
 // Override logging mechanism for non-R interfaces
 void dmlc::CustomLogMessage::Log(const std::string& msg) {
-  const xgboost::LogCallbackRegistry* registry
-    = xgboost::LogCallbackRegistryStore::Get();
+  const boxhed_kernel::LogCallbackRegistry* registry
+    = boxhed_kernel::LogCallbackRegistryStore::Get();
   auto callback = registry->Get();
   callback(msg.c_str());
 }
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 ConsoleLogger::~ConsoleLogger() {
   if (ShouldLog(cur_verbosity_)) {
     dmlc::CustomLogMessage::Log(BaseLogger::log_stream_.str());
   }
 }
 
 TrackerLogger::~TrackerLogger() {
   log_stream_ << '\n';
   rabit::TrackerPrint(log_stream_.str());
 }
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // !defined(XGBOOST_STRICT_R_MODE) || XGBOOST_STRICT_R_MODE == 0
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 DMLC_REGISTER_PARAMETER(ConsoleLoggerParam);
 
 ConsoleLogger::LogVerbosity ConsoleLogger::global_verbosity_ =
     ConsoleLogger::DefaultVerbosity();
 
 ConsoleLoggerParam ConsoleLogger::param_ = ConsoleLoggerParam();
@@ -102,8 +102,8 @@
       BaseLogger::log_stream_ << file << ":" << line << ": ";
       break;
     case LogVerbosity::kSilent:
       break;
   }
 }
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/metric/elementwise_metric.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/metric/elementwise_metric.cu`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  * \file elementwise_metric.cc
  * \brief evaluation metrics for elementwise binary or regression.
  * \author Kailong Chen, Tianqi Chen
  *
  *  The expressions like wsum == 0 ? esum : esum / wsum is used to handle empty dataset.
  */
 #include <rabit/rabit.h>
-#include <xgboost/metric.h>
+#include <boxhed_kernel/metric.h>
 #include <dmlc/registry.h>
 #include <cmath>
 
 #include "metric_common.h"
 #include "../common/math.h"
 #include "../common/common.h"
 
@@ -20,15 +20,15 @@
 #include <thrust/functional.h>        // thrust::plus<>
 #include <thrust/transform_reduce.h>
 #include <thrust/iterator/counting_iterator.h>
 
 #include "../common/device_helpers.cuh"
 #endif  // XGBOOST_USE_CUDA
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace metric {
 // tag the this file, used by force static link later.
 DMLC_REGISTRY_FILE_TAG(elementwise_metric);
 
 template <typename EvalRow>
 class ElementWiseMetricsReduction {
  public:
@@ -412,8 +412,8 @@
 XGBOOST_REGISTER_METRIC(TweedieNLogLik, "tweedie-nloglik")
 .describe("tweedie-nloglik@rho for tweedie regression.")
 .set_body([](const char* param) {
   return new EvalEWiseBase<EvalTweedieNLogLik>(param);
 });
 
 }  // namespace metric
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/metric/metric.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/metric/metric.cc`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /*!
  * Copyright 2015-2020 by Contributors
  * \file metric_registry.cc
  * \brief Registry of objective functions.
  */
 #include <dmlc/registry.h>
-#include <xgboost/metric.h>
-#include <xgboost/generic_parameters.h>
+#include <boxhed_kernel/metric.h>
+#include <boxhed_kernel/generic_parameters.h>
 
 #include "metric_common.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 template <typename MetricRegistry>
 Metric* CreateMetricImpl(const std::string& name) {
   std::string buf = name;
   std::string prefix = name;
   const char* param;
   auto pos = buf.find('@');
   if (pos == std::string::npos) {
@@ -64,26 +64,26 @@
 
   // Narrowing reference only for the compiler to allow assignment to a base class member.
   // As such, using this narrowed reference to refer to derived members will be an illegal op.
   // This is moot, as this type is stateless.
   static_cast<GPUMetric *>(metric)->tparam_ = tparam;
   return metric;
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 namespace dmlc {
-DMLC_REGISTRY_ENABLE(::xgboost::MetricReg);
-DMLC_REGISTRY_ENABLE(::xgboost::MetricGPUReg);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::MetricReg);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::MetricGPUReg);
 }
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace metric {
 // List of files that will be force linked in static links.
 DMLC_REGISTRY_LINK_TAG(elementwise_metric);
 DMLC_REGISTRY_LINK_TAG(multiclass_metric);
 DMLC_REGISTRY_LINK_TAG(survival_metric);
 DMLC_REGISTRY_LINK_TAG(rank_metric);
 #ifdef XGBOOST_USE_CUDA
 DMLC_REGISTRY_LINK_TAG(rank_metric_gpu);
 #endif
 }  // namespace metric
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/metric/metric_common.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/metric/metric_common.h`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 #define XGBOOST_METRIC_METRIC_COMMON_H_
 
 #include <limits>
 #include <string>
 
 #include "../common/common.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 // This creates a GPU metric instance dynamically and adds it to the GPU metric registry, if not
-// present already. This is created when there is a device ordinal present and if xgboost
+// present already. This is created when there is a device ordinal present and if boxhed_kernel
 // is compiled with CUDA support
 struct GPUMetric : Metric {
   static Metric *CreateGPUMetric(const std::string& name, GenericParameter const* tparam);
 };
 
 /*!
  * \brief Internal registry entries for GPU Metric factory functions.
@@ -42,16 +42,16 @@
  *   });
  * \endcode
  */
 
 // Note: Metric names registered in the GPU registry should follow this convention:
 // - GPU metric types should be registered with the same name as the non GPU metric types
 #define XGBOOST_REGISTER_GPU_METRIC(UniqueId, Name)                         \
-  ::xgboost::MetricGPUReg&  __make_ ## MetricGPUReg ## _ ## UniqueId ## __ =  \
-      ::dmlc::Registry< ::xgboost::MetricGPUReg>::Get()->__REGISTER__(Name)
+  ::boxhed_kernel::MetricGPUReg&  __make_ ## MetricGPUReg ## _ ## UniqueId ## __ =  \
+      ::dmlc::Registry< ::boxhed_kernel::MetricGPUReg>::Get()->__REGISTER__(Name)
 
 namespace metric {
 
 // Ranking config to be used on device and host
 struct EvalRankConfig {
  public:
   // Parsed from metric name, the top-n number of instances within a group after
@@ -81,10 +81,10 @@
     return *this;
   }
   double Residue() const { return residue_sum_; }
   double Weights() const { return weights_sum_; }
 };
 
 }  // namespace metric
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_METRIC_METRIC_COMMON_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/metric/multiclass_metric.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/metric/multiclass_metric.cu`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /*!
  * Copyright 2015-2019 by Contributors
  * \file multiclass_metric.cc
  * \brief evaluation metrics for multiclass classification.
  * \author Kailong Chen, Tianqi Chen
  */
 #include <rabit/rabit.h>
-#include <xgboost/metric.h>
+#include <boxhed_kernel/metric.h>
 #include <cmath>
 
 #include "metric_common.h"
 #include "../common/math.h"
 #include "../common/common.h"
 
 #if defined(XGBOOST_USE_CUDA)
@@ -17,15 +17,15 @@
 #include <thrust/functional.h>        // thrust::plus<>
 #include <thrust/transform_reduce.h>
 #include <thrust/iterator/counting_iterator.h>
 
 #include "../common/device_helpers.cuh"
 #endif  // XGBOOST_USE_CUDA
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace metric {
 // tag the this file, used by force static link later.
 DMLC_REGISTRY_FILE_TAG(multiclass_metric);
 
 template <typename EvalRowPolicy>
 class MultiClassMetricsReduction {
   void CheckLabelError(int32_t label_error, size_t n_class) const {
@@ -238,8 +238,8 @@
 .describe("Multiclass classification error.")
 .set_body([](const char* param) { return new EvalMatchError(); });
 
 XGBOOST_REGISTER_METRIC(MultiLogLoss, "mlogloss")
 .describe("Multiclass negative loglikelihood.")
 .set_body([](const char* param) { return new EvalMultiLogLoss(); });
 }  // namespace metric
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/metric/rank_metric.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/metric/rank_metric.cc`

 * *Files 3% similar despite different names*

```diff
@@ -6,38 +6,38 @@
 // for an invalid device ordinal to be specified in GPU builds - to train/predict and/or compute
 // the metrics on CPU. To accommodate these scenarios, the following is done for the metrics
 // accelarated on the GPU.
 // - An internal GPU registry holds all the GPU metric types (defined in the .cu file)
 // - An instance of the appropriate gpu metric type is created when a device ordinal is present
 // - If the creation is successful, the metric computation is done on the device
 // - else, it falls back on the CPU
-// - The GPU metric types are *only* registered when xgboost is built for GPUs
+// - The GPU metric types are *only* registered when boxhed_kernel is built for GPUs
 //
 // This is done for 2 reasons:
 // - Clear separation of CPU and GPU logic
 // - Sorting datasets containing large number of rows is (much) faster when parallel sort
 //   semantics is used on the CPU. The __gnu_parallel/concurrency primitives needed to perform
 //   this cannot be used when the translation unit is compiled using the 'nvcc' compiler (as the
 //   corresponding headers that brings in those function declaration can't be included with CUDA).
 //   This precludes the CPU and GPU logic to coexist inside a .cu file
 
 #include <rabit/rabit.h>
-#include <xgboost/metric.h>
+#include <boxhed_kernel/metric.h>
 #include <dmlc/registry.h>
 #include <cmath>
 
 #include <vector>
 
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/host_device_vector.h"
 #include "../common/math.h"
 #include "metric_common.h"
 
 namespace {
 
-using PredIndPair = std::pair<xgboost::bst_float, uint32_t>;
+using PredIndPair = std::pair<boxhed_kernel::bst_float, uint32_t>;
 using PredIndPairContainer = std::vector<PredIndPair>;
 
 /*
  * Adapter to access instance weights.
  *
  *  - For ranking task, weights are per-group
  *  - For binary classification task, weights are per-instance
@@ -49,46 +49,46 @@
  *   get weight associated with an individual instance, using index into
  *   sorted records `rec` (in ascending order of predicted labels). `rec` is
  *   of type PredIndPairContainer
  */
 
 class PerInstanceWeightPolicy {
  public:
-  inline static xgboost::bst_float
-  GetWeightOfInstance(const xgboost::MetaInfo& info,
+  inline static boxhed_kernel::bst_float
+  GetWeightOfInstance(const boxhed_kernel::MetaInfo& info,
                       unsigned instance_id, unsigned) {
     return info.GetWeight(instance_id);
   }
-  inline static xgboost::bst_float
-  GetWeightOfSortedRecord(const xgboost::MetaInfo& info,
+  inline static boxhed_kernel::bst_float
+  GetWeightOfSortedRecord(const boxhed_kernel::MetaInfo& info,
                           const PredIndPairContainer& rec,
                           unsigned record_id, unsigned) {
     return info.GetWeight(rec[record_id].second);
   }
 };
 
 class PerGroupWeightPolicy {
  public:
-  inline static xgboost::bst_float
-  GetWeightOfInstance(const xgboost::MetaInfo& info,
+  inline static boxhed_kernel::bst_float
+  GetWeightOfInstance(const boxhed_kernel::MetaInfo& info,
                       unsigned, unsigned group_id) {
     return info.GetWeight(group_id);
   }
 
-  inline static xgboost::bst_float
-  GetWeightOfSortedRecord(const xgboost::MetaInfo& info,
+  inline static boxhed_kernel::bst_float
+  GetWeightOfSortedRecord(const boxhed_kernel::MetaInfo& info,
                           const PredIndPairContainer&,
                           unsigned, unsigned group_id) {
     return info.GetWeight(group_id);
   }
 };
 
 }  // anonymous namespace
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace metric {
 // tag the this file, used by force static link later.
 DMLC_REGISTRY_FILE_TAG(rank_metric);
 
 /*! \brief AMS: also records best threshold */
 struct EvalAMS : public Metric {
  public:
@@ -157,15 +157,15 @@
 };
 
 /*! \brief Area Under Curve, for both classification and rank computed on CPU */
 struct EvalAuc : public Metric {
  private:
   // This is used to compute the AUC metrics on the GPU - for ranking tasks and
   // for training jobs that run on the GPU.
-  std::unique_ptr<xgboost::Metric> auc_gpu_;
+  std::unique_ptr<boxhed_kernel::Metric> auc_gpu_;
 
   template <typename WeightPolicy>
   bst_float Eval(const HostDeviceVector<bst_float> &preds,
                  const MetaInfo &info,
                  bool distributed,
                  const std::vector<unsigned> &gptr) {
     const auto ngroups = static_cast<bst_omp_uint>(gptr.size() - 1);
@@ -276,15 +276,15 @@
   const char *Name() const override { return "auc"; }
 };
 
 /*! \brief Evaluate rank list */
 struct EvalRank : public Metric, public EvalRankConfig {
  private:
   // This is used to compute the ranking metrics on the GPU - for training jobs that run on the GPU.
-  std::unique_ptr<xgboost::Metric> rank_gpu_;
+  std::unique_ptr<boxhed_kernel::Metric> rank_gpu_;
 
  public:
   bst_float Eval(const HostDeviceVector<bst_float> &preds,
                  const MetaInfo &info,
                  bool distributed) override {
     CHECK_EQ(preds.Size(), info.labels_.Size())
         << "label size predict size not match";
@@ -506,15 +506,15 @@
 struct EvalAucPR : public Metric {
   // implementation of AUC-PR for weighted data
   // translated from PRROC R Package
   // see https://doi.org/10.1371/journal.pone.0092209
  private:
   // This is used to compute the AUCPR metrics on the GPU - for ranking tasks and
   // for training jobs that run on the GPU.
-  std::unique_ptr<xgboost::Metric> aucpr_gpu_;
+  std::unique_ptr<boxhed_kernel::Metric> aucpr_gpu_;
 
   template <typename WeightPolicy>
   bst_float Eval(const HostDeviceVector<bst_float> &preds,
                  const MetaInfo &info,
                  bool distributed,
                  const std::vector<unsigned> &gptr) {
     const auto ngroups = static_cast<bst_omp_uint>(gptr.size() - 1);
@@ -669,8 +669,8 @@
 .describe("map@k for rank.")
 .set_body([](const char* param) { return new EvalMAP("map", param); });
 
 XGBOOST_REGISTER_METRIC(Cox, "cox-nloglik")
 .describe("Negative log partial likelihood of Cox proportioanl hazards model.")
 .set_body([](const char*) { return new EvalCox(); });
 }  // namespace metric
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/metric/rank_metric.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/metric/rank_metric.cu`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
  * \file rank_metric.cc
  * \brief prediction rank based metrics.
  * \author Kailong Chen, Tianqi Chen
  */
 #include <rabit/rabit.h>
 #include <dmlc/registry.h>
 
-#include <xgboost/metric.h>
-#include <xgboost/host_device_vector.h>
+#include <boxhed_kernel/metric.h>
+#include <boxhed_kernel/host_device_vector.h>
 #include <thrust/iterator/discard_iterator.h>
 
 #include <cmath>
 #include <array>
 #include <vector>
 
 #include "metric_common.h"
 
 #include "../common/math.h"
 #include "../common/device_helpers.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace metric {
 // tag the this file, used by force static link later.
 DMLC_REGISTRY_FILE_TAG(rank_metric_gpu);
 
 /*! \brief Evaluate rank list on GPU */
 template <typename EvalMetricT>
 struct EvalRankGpu : public Metric, public EvalRankConfig {
@@ -127,15 +127,15 @@
 struct EvalNDCGGpu {
  public:
   static void ComputeDCG(const dh::SegmentSorter<float> &pred_sorter,
                          const float *dlabels,
                          const EvalRankConfig &ecfg,
                          // The order in which labels have to be accessed. The order is determined
                          // by sorting the predictions or the labels for the entire dataset
-                         const xgboost::common::Span<const uint32_t> &dlabels_sort_order,
+                         const boxhed_kernel::common::Span<const uint32_t> &dlabels_sort_order,
                          dh::caching_device_vector<double> *dcgptr) {
     dh::caching_device_vector<double> &dcgs(*dcgptr);
     // Group info on device
     const auto &dgroups = pred_sorter.GetGroupsSpan();
     const auto &dgroup_idx = pred_sorter.GetGroupSegmentsSpan();
 
     // First, determine non zero labels in the dataset individually
@@ -516,15 +516,15 @@
       kPositive,
       kNegative
     };
 
     XGBOOST_DEVICE ComputeItemPrecision(PrecisionType ptype,
                                         uint32_t ngroups,
                                         const float *dweights,
-                                        const xgboost::common::Span<const uint32_t> &dgidxs,
+                                        const boxhed_kernel::common::Span<const uint32_t> &dgidxs,
                                         const float *dlabels)
       : ptype_(ptype), ngroups_(ngroups), dweights_(dweights), dgidxs_(dgidxs), dlabels_(dlabels) {}
 
     // Compute precision value for the prediction that was originally at 'idx'
     __device__ __forceinline__ float operator()(uint32_t idx) const {
       // For ranking task, weights are per-group
       // For binary classification task, weights are per-instance
@@ -532,15 +532,15 @@
       return wt * (ptype_ == PrecisionType::kPositive ? dlabels_[idx] : (1.0f - dlabels_[idx]));
     }
 
    private:
     PrecisionType ptype_;  // Precision type to be computed
     uint32_t ngroups_;  // Number of groups in the dataset
     const float *dweights_;  // Instance/group weights
-    const xgboost::common::Span<const uint32_t> dgidxs_;  // The group a given instance belongs to
+    const boxhed_kernel::common::Span<const uint32_t> dgidxs_;  // The group a given instance belongs to
     const float *dlabels_;  // Unsorted labels in the dataset
   };
 
   bst_float Eval(const HostDeviceVector<bst_float> &preds,
                  const MetaInfo &info,
                  bool distributed) override {
     // Sanity check is done by the caller
@@ -707,8 +707,8 @@
 .describe("ndcg@k for rank computed on GPU.")
 .set_body([](const char* param) { return new EvalRankGpu<EvalNDCGGpu>("ndcg", param); });
 
 XGBOOST_REGISTER_GPU_METRIC(MAPGpu, "map")
 .describe("map@k for rank computed on GPU.")
 .set_body([](const char* param) { return new EvalRankGpu<EvalMAPGpu>("map", param); });
 }  // namespace metric
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/metric/survival_metric.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/metric/survival_metric.cu`

 * *Files 6% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 
 #include <rabit/rabit.h>
 #include <dmlc/registry.h>
 
 #include <memory>
 #include <vector>
 
-#include "xgboost/json.h"
-#include "xgboost/metric.h"
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/metric.h"
+#include "boxhed_kernel/host_device_vector.h"
 
 #include "metric_common.h"
 #include "../common/math.h"
 #include "../common/survival_util.h"
 
 #if defined(XGBOOST_USE_CUDA)
 #include <thrust/execution_policy.h>  // thrust::cuda::par
 #include "../common/device_helpers.cuh"
 #endif  // XGBOOST_USE_CUDA
 
-using AFTParam = xgboost::common::AFTParam;
-using ProbabilityDistributionType = xgboost::common::ProbabilityDistributionType;
+using AFTParam = boxhed_kernel::common::AFTParam;
+using ProbabilityDistributionType = boxhed_kernel::common::ProbabilityDistributionType;
 template <typename Distribution>
-using AFTLoss = xgboost::common::AFTLoss<Distribution>;
+using AFTLoss = boxhed_kernel::common::AFTLoss<Distribution>;
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace metric {
 // tag the this file, used by force static link later.
 DMLC_REGISTRY_FILE_TAG(survival_metric);
 
 template <typename EvalRow>
 class ElementWiseSurvivalMetricsReduction {
  public:
@@ -293,8 +293,8 @@
 XGBOOST_REGISTER_METRIC(IntervalRegressionAccuracy, "interval-regression-accuracy")
 .describe("")
 .set_body([](const char* param) {
   return new EvalEWiseSurvivalBase<EvalIntervalRegressionAccuracy>();
 });
 
 }  // namespace metric
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/objective/aft_obj.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/objective/aft_obj.cu`

 * *Files 5% similar despite different names*

```diff
@@ -6,30 +6,30 @@
  */
 
 #include <vector>
 #include <limits>
 #include <memory>
 #include <utility>
 
-#include "xgboost/host_device_vector.h"
-#include "xgboost/json.h"
-#include "xgboost/parameter.h"
-#include "xgboost/span.h"
-#include "xgboost/logging.h"
-#include "xgboost/objective.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/span.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/objective.h"
 
 #include "../common/transform.h"
 #include "../common/survival_util.h"
 
-using AFTParam = xgboost::common::AFTParam;
-using ProbabilityDistributionType = xgboost::common::ProbabilityDistributionType;
+using AFTParam = boxhed_kernel::common::AFTParam;
+using ProbabilityDistributionType = boxhed_kernel::common::ProbabilityDistributionType;
 template <typename Distribution>
-using AFTLoss = xgboost::common::AFTLoss<Distribution>;
+using AFTLoss = boxhed_kernel::common::AFTLoss<Distribution>;
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 
 #if defined(XGBOOST_USE_CUDA)
 DMLC_REGISTRY_FILE_TAG(aft_obj_gpu);
 #endif  // defined(XGBOOST_USE_CUDA)
 
 class AFTObj : public ObjFunction {
@@ -140,8 +140,8 @@
 
 // register the objective functions
 XGBOOST_REGISTER_OBJECTIVE(AFTObj, "survival:aft")
     .describe("AFT loss function")
     .set_body([]() { return new AFTObj(); });
 
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/objective/hinge.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/objective/hinge.cu`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 /*!
  * Copyright 2018-2019 by Contributors
  * \file hinge.cc
  * \brief Provides an implementation of the hinge loss function
  * \author Henry Gouk
  */
-#include "xgboost/objective.h"
-#include "xgboost/json.h"
-#include "xgboost/span.h"
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/objective.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/span.h"
+#include "boxhed_kernel/host_device_vector.h"
 
 #include "../common/math.h"
 #include "../common/transform.h"
 #include "../common/common.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 
 #if defined(XGBOOST_USE_CUDA)
 DMLC_REGISTRY_FILE_TAG(hinge_obj_gpu);
 #endif  // defined(XGBOOST_USE_CUDA)
 
 class HingeObj : public ObjFunction {
@@ -91,8 +91,8 @@
 
 // register the objective functions
 XGBOOST_REGISTER_OBJECTIVE(HingeObj, "binary:hinge")
 .describe("Hinge loss. Expects labels to be in [0,1f]")
 .set_body([]() { return new HingeObj(); });
 
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/objective/multiclass_obj.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/objective/multiclass_obj.cu`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 #include <dmlc/omp.h>
 
 #include <vector>
 #include <algorithm>
 #include <limits>
 #include <utility>
 
-#include "xgboost/parameter.h"
-#include "xgboost/data.h"
-#include "xgboost/logging.h"
-#include "xgboost/objective.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/objective.h"
+#include "boxhed_kernel/json.h"
 
 #include "../common/common.h"
 #include "../common/math.h"
 #include "../common/transform.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 
 #if defined(XGBOOST_USE_CUDA)
 DMLC_REGISTRY_FILE_TAG(multiclass_obj_gpu);
 #endif  // defined(XGBOOST_USE_CUDA)
 
 struct SoftmaxMultiClassParam : public XGBoostParameter<SoftmaxMultiClassParam> {
@@ -200,8 +200,8 @@
 .set_body([]() { return new SoftmaxMultiClassObj(false); });
 
 XGBOOST_REGISTER_OBJECTIVE(SoftprobMultiClass, "multi:softprob")
 .describe("Softmax for multi-class classification, output probability distribution.")
 .set_body([]() { return new SoftmaxMultiClassObj(true); });
 
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/objective/objective.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/objective/objective.cc`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 /*!
  * Copyright 2015 by Contributors
  * \file objective.cc
  * \brief Registry of all objective functions.
  */
-#include <xgboost/objective.h>
+#include <boxhed_kernel/objective.h>
 #include <dmlc/registry.h>
 
 #include <sstream>
 
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/host_device_vector.h"
 
 namespace dmlc {
-DMLC_REGISTRY_ENABLE(::xgboost::ObjFunctionReg);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::ObjFunctionReg);
 }  // namespace dmlc
 
-namespace xgboost {
+namespace boxhed_kernel {
 // implement factory functions
 ObjFunction* ObjFunction::Create(const std::string& name, GenericParameter const* tparam) {
-  auto *e = ::dmlc::Registry< ::xgboost::ObjFunctionReg>::Get()->Find(name);
+  auto *e = ::dmlc::Registry< ::boxhed_kernel::ObjFunctionReg>::Get()->Find(name);
   if (e == nullptr) {
     std::stringstream ss;
-    for (const auto& entry : ::dmlc::Registry< ::xgboost::ObjFunctionReg>::List()) {
+    for (const auto& entry : ::dmlc::Registry< ::boxhed_kernel::ObjFunctionReg>::List()) {
       ss << "Objective candidate: " << entry->name << "\n";
     }
     LOG(FATAL) << "Unknown objective function: `" << name << "`\n"
                << ss.str();
   }
   auto pobj = (e->body)();
   pobj->tparam_ = tparam;
   return pobj;
 }
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 // List of files that will be force linked in static links.
 #ifdef XGBOOST_USE_CUDA
 DMLC_REGISTRY_LINK_TAG(regression_obj_gpu);
 DMLC_REGISTRY_LINK_TAG(hinge_obj_gpu);
 DMLC_REGISTRY_LINK_TAG(multiclass_obj_gpu);
 DMLC_REGISTRY_LINK_TAG(rank_obj_gpu);
 #else
 DMLC_REGISTRY_LINK_TAG(regression_obj);
 DMLC_REGISTRY_LINK_TAG(hinge_obj);
 DMLC_REGISTRY_LINK_TAG(multiclass_obj);
 DMLC_REGISTRY_LINK_TAG(rank_obj);
 #endif  // XGBOOST_USE_CUDA
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/objective/rank_obj.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/objective/rank_obj.cu`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 /*!
  * Copyright 2015-2019 XGBoost contributors
  */
 #include <dmlc/omp.h>
 #include <dmlc/timer.h>
-#include <xgboost/logging.h>
-#include <xgboost/objective.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/objective.h>
 #include <vector>
 #include <algorithm>
 #include <utility>
 
-#include "xgboost/json.h"
-#include "xgboost/parameter.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/parameter.h"
 
 #include "../common/math.h"
 #include "../common/random.h"
 
 #if defined(__CUDACC__)
 #include <thrust/sort.h>
 #include <thrust/gather.h>
@@ -23,15 +23,15 @@
 #include <thrust/random/linear_congruential_engine.h>
 
 #include <cub/util_allocator.cuh>
 
 #include "../common/device_helpers.cuh"
 #endif
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 
 #if defined(XGBOOST_USE_CUDA) && !defined(GTEST_TEST)
 DMLC_REGISTRY_FILE_TAG(rank_obj_gpu);
 #endif  // defined(XGBOOST_USE_CUDA)
 
 struct LambdaRankParam : public XGBoostParameter<LambdaRankParam> {
@@ -947,8 +947,8 @@
 
 XGBOOST_REGISTER_OBJECTIVE(LambdaRankObjMAP, MAPLambdaWeightComputer::Name())
 .describe("LambdaRank with MAP as objective.")
 .set_body([]() { return new LambdaRankObj<MAPLambdaWeightComputer>(); });
 #endif
 
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/objective/regression_loss.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/objective/regression_loss.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /*!
  * Copyright 2017-2019 XGBoost contributors
  */
 #ifndef XGBOOST_OBJECTIVE_REGRESSION_LOSS_H_
 #define XGBOOST_OBJECTIVE_REGRESSION_LOSS_H_
 
 #include <dmlc/omp.h>
-#include <xgboost/logging.h>
+#include <boxhed_kernel/logging.h>
 #include <algorithm>
 #include "../common/math.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 
 // common regressions
 // linear regression
 struct LinearSquareLoss {
   // duplication is necessary, as __device__ specifier
   // cannot be made conditional on template parameter
@@ -164,10 +164,10 @@
   }
   static const char* DefaultEvalMetric() { return "auc"; }
 
   static const char* Name() { return "binary:logitraw"; }
 };
 
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_OBJECTIVE_REGRESSION_LOSS_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/objective/regression_obj.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/objective/regression_obj.cu`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,31 @@
  * Copyright 2015-2019 by Contributors
  * \file regression_obj.cu
  * \brief Definition of single-value regression and classification objectives.
  * \author Tianqi Chen, Kailong Chen
  */
 
 #include <dmlc/omp.h>
-#include <xgboost/logging.h>
-#include <xgboost/objective.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/objective.h>
 #include <cmath>
 #include <memory>
 #include <vector>
 
-#include "xgboost/host_device_vector.h"
-#include "xgboost/json.h"
-#include "xgboost/parameter.h"
-#include "xgboost/span.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/span.h"
 
 #include "../common/transform.h"
 #include "../common/common.h"
 #include "./regression_loss.h"
 
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace obj {
 
 #if defined(XGBOOST_USE_CUDA)
 DMLC_REGISTRY_FILE_TAG(regression_obj_gpu);
 #endif  // defined(XGBOOST_USE_CUDA)
 
 struct RegLossParam : public XGBoostParameter<RegLossParam> {
@@ -704,8 +704,8 @@
 DMLC_REGISTER_PARAMETER(TweedieRegressionParam);
 
 XGBOOST_REGISTER_OBJECTIVE(TweedieRegression, "reg:tweedie")
 .describe("Tweedie regression for insurance data.")
 .set_body([]() { return new TweedieRegression(); });
 
 }  // namespace obj
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/predictor/cpu_predictor.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/predictor/cpu_predictor.cc`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 #include <dmlc/omp.h>
 #include <dmlc/any.h>
 
 #include <cstddef>
 #include <limits>
 #include <mutex>
 
-#include "xgboost/base.h"
-#include "xgboost/data.h"
-#include "xgboost/predictor.h"
-#include "xgboost/tree_model.h"
-#include "xgboost/tree_updater.h"
-#include "xgboost/logging.h"
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/predictor.h"
+#include "boxhed_kernel/tree_model.h"
+#include "boxhed_kernel/tree_updater.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/host_device_vector.h"
 
 #include "../data/adapter.h"
 #include "../common/math.h"
 #include "../gbm/gbtree_model.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace predictor {
 
 DMLC_REGISTRY_FILE_TAG(cpu_predictor);
 
 bst_float PredValue(const SparsePage::Inst &inst,
                     const std::vector<std::unique_ptr<RegTree>> &trees,
                     const std::vector<int> &tree_info, int bst_group,
@@ -506,8 +506,8 @@
 
 XGBOOST_REGISTER_PREDICTOR(CPUPredictor, "cpu_predictor")
 .describe("Make predictions using CPU.")
 .set_body([](GenericParameter const* generic_param) {
             return new CPUPredictor(generic_param);
           });
 }  // namespace predictor
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/predictor/gpu_predictor.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/predictor/gpu_predictor.cu`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 #include <thrust/copy.h>
 #include <thrust/device_ptr.h>
 #include <thrust/device_vector.h>
 #include <thrust/fill.h>
 #include <GPUTreeShap/gpu_treeshap.h>
 #include <memory>
 
-#include "xgboost/data.h"
-#include "xgboost/predictor.h"
-#include "xgboost/tree_model.h"
-#include "xgboost/tree_updater.h"
-#include "xgboost/host_device_vector.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/predictor.h"
+#include "boxhed_kernel/tree_model.h"
+#include "boxhed_kernel/tree_updater.h"
+#include "boxhed_kernel/host_device_vector.h"
 
 #include "../gbm/gbtree_model.h"
 #include "../data/ellpack_page.cuh"
 #include "../data/device_adapter.cuh"
 #include "../common/common.h"
 #include "../common/bitfield.h"
 #include "../common/categorical.h"
 #include "../common/device_helpers.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace predictor {
 
 DMLC_REGISTRY_FILE_TAG(gpu_predictor);
 
 struct SparsePageView {
   common::Span<const Entry> d_data;
   common::Span<const bst_row_t> d_row_ptr;
@@ -490,15 +490,15 @@
   if (shared_memory_bytes > max_shared_memory_bytes) {
     shared_memory_bytes = 0;
   }
   return shared_memory_bytes;
 }
 }  // anonymous namespace
 
-class GPUPredictor : public xgboost::Predictor {
+class GPUPredictor : public boxhed_kernel::Predictor {
  private:
   void PredictInternal(const SparsePage& batch,
                        size_t num_features,
                        HostDeviceVector<bst_float>* predictions,
                        size_t batch_offset) {
     batch.offset.SetDevice(generic_param_->gpu_id);
     batch.data.SetDevice(generic_param_->gpu_id);
@@ -910,8 +910,8 @@
 XGBOOST_REGISTER_PREDICTOR(GPUPredictor, "gpu_predictor")
 .describe("Make predictions using GPU.")
 .set_body([](GenericParameter const* generic_param) {
             return new GPUPredictor(generic_param);
           });
 
 }  // namespace predictor
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/predictor/predictor.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/predictor/predictor.cc`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /*!
  * Copyright 2017-2020 by Contributors
  */
 #include <dmlc/registry.h>
 #include <mutex>
 
-#include "xgboost/predictor.h"
-#include "xgboost/data.h"
-#include "xgboost/generic_parameters.h"
+#include "boxhed_kernel/predictor.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/generic_parameters.h"
 
 namespace dmlc {
-DMLC_REGISTRY_ENABLE(::xgboost::PredictorReg);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::PredictorReg);
 }  // namespace dmlc
 
-namespace xgboost {
+namespace boxhed_kernel {
 void PredictionContainer::ClearExpiredEntries() {
   std::vector<DMatrix*> expired;
   for (auto& kv : container_) {
     if (kv.second.ref.expired()) {
       expired.emplace_back(kv.first);
     }
   }
@@ -54,18 +54,18 @@
   auto* e = ::dmlc::Registry<PredictorReg>::Get()->Find(name);
   if (e == nullptr) {
     LOG(FATAL) << "Unknown predictor type " << name;
   }
   auto p_predictor = (e->body)(generic_param);
   return p_predictor;
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace predictor {
 // List of files that will be force linked in static links.
 #ifdef XGBOOST_USE_CUDA
 DMLC_REGISTRY_LINK_TAG(gpu_predictor);
 #endif  // XGBOOST_USE_CUDA
 DMLC_REGISTRY_LINK_TAG(cpu_predictor);
 }  // namespace predictor
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/constraints.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/constraints.cc`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 /*!
  * Copyright 2018-2019 by Contributors
  */
 #include <algorithm>
 #include <unordered_set>
 #include <vector>
 
-#include "xgboost/span.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/span.h"
+#include "boxhed_kernel/json.h"
 #include "constraints.h"
 #include "param.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 void FeatureInteractionConstraintHost::Configure(tree::TrainParam const& param,
                                                  bst_feature_t const n_features) {
   if (param.interaction_constraints.empty()) {
     enabled_ = !param.interaction_constraints.empty();
     return;  // short-circuit if no constraint is specified
   }
   enabled_ = true;
@@ -96,8 +96,8 @@
       for (bst_uint k : constraint) {
         node_constraints_[left_id].insert(k);
         node_constraints_[right_id].insert(k);
       }
     }
   }
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/constraints.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/constraints.cu`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 #include <thrust/execution_policy.h>
 #include <thrust/iterator/counting_iterator.h>
 
 #include <algorithm>
 #include <string>
 #include <set>
 
-#include "xgboost/logging.h"
-#include "xgboost/span.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/span.h"
 #include "constraints.cuh"
 #include "param.h"
 #include "../common/device_helpers.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 size_t FeatureInteractionConstraintDevice::Features() const {
   return d_sets_ptr_.size() - 1;
 }
 
 void FeatureInteractionConstraintDevice::Configure(
     tree::TrainParam const& param, int32_t const n_features) {
@@ -328,8 +328,8 @@
   dh::LaunchKernel {n_grids, kBlockThreads} (
       InteractionConstraintSplitKernel,
       feature_buffer_,
       feature_id,
       node, left, right);
 }
 
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/constraints.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/constraints.cuh`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 #include <dmlc/json.h>
 
 #include <cinttypes>
 #include <vector>
 
 #include "param.h"
 #include "constraints.h"
-#include "xgboost/span.h"
+#include "boxhed_kernel/span.h"
 #include "../common/bitfield.h"
 #include "../common/device_helpers.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 // Feature interaction constraints built for GPU Hist updater.
 struct FeatureInteractionConstraintDevice {
  protected:
   // Whether interaction constraint is used.
   bool has_constraint_;
   // n interaction sets.
   size_t n_sets_;
@@ -91,9 +91,9 @@
    * node.
    */
   common::Span<bst_feature_t> Query(common::Span<bst_feature_t> feature_list, int32_t nid);
   /*! \brief Apply split for node_id. */
   void Split(bst_node_t node_id, bst_feature_t feature_id, bst_node_t left_id, bst_node_t right_id);
 };
 
-}      // namespace xgboost
+}      // namespace boxhed_kernel
 #endif  // XGBOOST_TREE_CONSTRAINTS_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/constraints.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/constraints.h`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 #ifndef XGBOOST_TREE_CONSTRAINTS_H_
 #define XGBOOST_TREE_CONSTRAINTS_H_
 
 #include <string>
 #include <unordered_set>
 #include <vector>
 
-#include "xgboost/span.h"
-#include "xgboost/base.h"
+#include "boxhed_kernel/span.h"
+#include "boxhed_kernel/base.h"
 
 #include "param.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 /*!
  * \brief Feature interaction constraint implementation for CPU tree updaters.
  *
  * The interface is similiar to the one for GPU Hist.
  */
 class FeatureInteractionConstraintHost {
  protected:
@@ -56,10 +56,10 @@
     return node_constraints_.at(nid).find(fid) != node_constraints_.at(nid).cend();
   }
 
   void Reset();
 
   void Configure(tree::TrainParam const& param, bst_feature_t const n_features);
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_TREE_CONSTRAINTS_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/driver.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/driver.cuh`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 /*!
  * Copyright 2020 by XGBoost Contributors
  */
 #ifndef DRIVER_CUH_
 #define DRIVER_CUH_
-#include <xgboost/span.h>
+#include <boxhed_kernel/span.h>
 #include <queue>
 #include "../param.h"
 #include "evaluate_splits.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 struct ExpandEntry {
   int nid;
   int depth;
   DeviceSplitCandidate split;
 
   float base_weight { std::numeric_limits<float>::quiet_NaN() };
@@ -118,10 +118,10 @@
   }
 
  private:
   TrainParam::TreeGrowPolicy policy_;
   ExpandQueue queue_;
 };
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // DRIVER_CUH_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/evaluate_splits.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/evaluate_splits.cu`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /*!
  * Copyright 2020 by XGBoost Contributors
  */
 #include <limits>
 #include "evaluate_splits.cuh"
 #include "../../common/categorical.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 // With constraints
 template <typename GradientPairT>
 XGBOOST_DEVICE float
 LossChangeMissing(const GradientPairT &scan, const GradientPairT &missing,
                   const GradientPairT &parent_sum,
@@ -335,8 +335,8 @@
     TreeEvaluator::SplitEvaluator<GPUTrainingParam> evaluator,
     EvaluateSplitInputs<GradientPair> input);
 template void EvaluateSingleSplit<GradientPairPrecise>(
     common::Span<DeviceSplitCandidate> out_split,
     TreeEvaluator::SplitEvaluator<GPUTrainingParam> evaluator,
     EvaluateSplitInputs<GradientPairPrecise> input);
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/feature_groups.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/feature_groups.cu`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /*!
  * Copyright 2020 by XGBoost Contributors
  */
 
-#include <xgboost/base.h>
+#include <boxhed_kernel/base.h>
 #include <algorithm>
 #include <vector>
 
 #include "feature_groups.cuh"
 
 #include "../../common/device_helpers.cuh"
 #include "../../common/hist_util.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 FeatureGroups::FeatureGroups(const common::HistogramCuts& cuts, bool is_dense,
                              size_t shm_size, size_t bin_size) {
   // Only use a single feature group for sparse matrices.
   bool single_group = !is_dense;
   if (single_group) {
@@ -57,8 +57,8 @@
   bin_segments_h.push_back(0);
   bin_segments_h.push_back(cuts.TotalBins());
 
   max_group_bins = cuts.TotalBins();
 }
 
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/feature_groups.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/feature_groups.cuh`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 /*!
  * Copyright 2020 by XGBoost Contributors
  */
 #ifndef FEATURE_GROUPS_CUH_
 #define FEATURE_GROUPS_CUH_
 
-#include <xgboost/host_device_vector.h>
-#include <xgboost/span.h>
+#include <boxhed_kernel/host_device_vector.h>
+#include <boxhed_kernel/span.h>
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 // Forward declarations.
 namespace common {
 class HistogramCuts;
 }  // namespace common
 
 namespace tree {
@@ -110,10 +110,10 @@
   }
 
 private:
   void InitSingle(const common::HistogramCuts& cuts);
 }; 
 
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // FEATURE_GROUPS_CUH_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cu`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /*!
  * Copyright 2019 by XGBoost Contributors
  */
 #include <thrust/functional.h>
 #include <thrust/random.h>
 #include <thrust/transform.h>
-#include <xgboost/host_device_vector.h>
-#include <xgboost/logging.h>
+#include <boxhed_kernel/host_device_vector.h>
+#include <boxhed_kernel/logging.h>
 
 #include <algorithm>
 #include <limits>
 
 #include "../../common/compressed_iterator.h"
 #include "../../common/random.h"
 #include "gradient_based_sampler.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 /*! \brief A functor that returns random weights. */
 class RandomWeight : public thrust::unary_function<size_t, float> {
  public:
   explicit RandomWeight(size_t seed) : seed_(seed) {}
 
@@ -375,8 +375,8 @@
                     SampleRateDelta(threshold, gpair.size(), sample_rows));
   thrust::device_ptr<float> min =
       thrust::min_element(dh::tbegin(grad_sum), dh::tend(grad_sum));
   return thrust::distance(dh::tbegin(grad_sum), min) + 1;
 }
 
 };  // namespace tree
-};  // namespace xgboost
+};  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cuh`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /*!
  * Copyright 2019 by XGBoost Contributors
  */
 #pragma once
-#include <xgboost/base.h>
-#include <xgboost/data.h>
-#include <xgboost/span.h>
+#include <boxhed_kernel/base.h>
+#include <boxhed_kernel/data.h>
+#include <boxhed_kernel/span.h>
 
 #include "../../common/device_helpers.cuh"
 #include "../../data/ellpack_page.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 struct GradientBasedSample {
   /*!\brief Number of sampled rows. */
   size_t sample_rows;
   /*!\brief Sampled rows in ELLPACK format. */
   EllpackPageImpl* page;
@@ -144,8 +144,8 @@
                                         size_t sample_rows);
 
  private:
   common::Monitor monitor_;
   std::unique_ptr<SamplingStrategy> strategy_;
 };
 };  // namespace tree
-};  // namespace xgboost
+};  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/histogram.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/histogram.cu`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
  */
 #include <thrust/reduce.h>
 #include <thrust/iterator/transform_iterator.h>
 #include <algorithm>
 #include <ctgmath>
 #include <limits>
 
-#include "xgboost/base.h"
+#include "boxhed_kernel/base.h"
 #include "row_partitioner.cuh"
 
 #include "histogram.cuh"
 
 #include "../../data/ellpack_page.cuh"
 #include "../../common/device_helpers.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 // Following 2 functions are slightly modifed version of fbcuda.
 
 /* \brief Constructs a rounding factor used to truncate elements in a sum such that the
    sum of the truncated elements is the same no matter what the order of the sum is.
 
  * Algorithm 5: Reproducible Sequential Sum in 'Fast Reproducible Floating-Point
@@ -224,8 +224,8 @@
     FeatureGroupsAccessor const& feature_groups,
     common::Span<GradientPair const> gpair,
     common::Span<const uint32_t> ridx,
     common::Span<GradientPairPrecise> histogram,
     GradientPairPrecise rounding);
 
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/row_partitioner.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/row_partitioner.cu`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #include <thrust/iterator/discard_iterator.h>
 #include <thrust/iterator/transform_output_iterator.h>
 #include <thrust/sequence.h>
 #include <vector>
 #include "../../common/device_helpers.cuh"
 #include "row_partitioner.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 struct IndicateLeftTransform {
   bst_node_t left_nidx;
   explicit IndicateLeftTransform(bst_node_t left_nidx) : left_nidx(left_nidx) {}
   __host__ __device__ __forceinline__ size_t
   operator()(const bst_node_t& x) const {
@@ -180,8 +180,8 @@
   const auto d_ridx_other = ridx_temp.data().get() + segment.begin;
   dh::LaunchN(device_idx_, segment.Size(), stream, [=] __device__(size_t idx) {
     d_position_current[idx] = d_position_other[idx];
     d_ridx_current[idx] = d_ridx_other[idx];
   });
 }
 };  // namespace tree
-};  // namespace xgboost
+};  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/gpu_hist/row_partitioner.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/gpu_hist/row_partitioner.cuh`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /*!
  * Copyright 2017-2019 XGBoost contributors
  */
 #pragma once
-#include "xgboost/base.h"
+#include "boxhed_kernel/base.h"
 #include "../../common/device_helpers.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 /*! \brief Count how many rows are assigned to left node. */
 __forceinline__ __device__ void AtomicIncrement(int64_t* d_count, bool increment) {
 #if __CUDACC_VER_MAJOR__ > 8
   int mask = __activemask();
   unsigned ballot = __ballot_sync(mask, increment);
@@ -186,8 +186,8 @@
     Segment(size_t begin, size_t end) : begin(begin), end(end) {
       CHECK_GE(end, begin);
     }
     size_t Size() const { return end - begin; }
   };
 };
 };  // namespace tree
-};  // namespace xgboost
+};  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/param.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/param.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /*!
  * Copyright by Contributors 2019
  */
 #include <iostream>
 #include <vector>
 #include <utility>
 
-#include "xgboost/json.h"
+#include "boxhed_kernel/json.h"
 #include "param.h"
 
 namespace std {
 std::istream &operator>>(std::istream &is, std::vector<int> &t) {
   t.clear();
   // get (
   while (true) {
@@ -77,15 +77,15 @@
     }
   }
   t = std::move(tmp);
   return is;
 }
 }  // namespace std
 
-namespace xgboost {
+namespace boxhed_kernel {
 void ParseInteractionConstraint(
     std::string const &constraint_str,
     std::vector<std::vector<bst_feature_t>> *p_out) {
   auto &out = *p_out;
   auto j_inc = Json::Load({constraint_str.c_str(), constraint_str.size()});
   auto const &all = get<Array>(j_inc);
   out.resize(all.size());
@@ -103,8 +103,8 @@
       } else {
         LOG(FATAL) << "Unknown value type for interaction constraint:"
                    << v.GetValue().TypeStr();
       }
     }
   }
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/param.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/param.h`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 #include <cmath>
 #include <cstring>
 #include <limits>
 #include <string>
 #include <vector>
 
-#include "xgboost/parameter.h"
-#include "xgboost/data.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/data.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 /*! \brief training parameters for regression tree */
 struct TrainParam : public XGBoostParameter<TrainParam> {
   // learning step size for a time
   float learning_rate;
   // minimum loss change required for a split
@@ -267,15 +267,15 @@
 template <typename T>
 XGBOOST_DEVICE inline static T Sqr(T a) { return a * a; }
 
 // calculate the cost of loss function
 template <typename TrainingParams, typename T>
 XGBOOST_DEVICE inline T CalcGainGivenWeight(const TrainingParams &p,
                                             T sum_grad, T sum_hess, T w) {
-  return ((sum_hess == T(0.0))||(sum_grad == T(0.0))) ? -std::numeric_limits<double>::infinity() : sum_hess * std::log(sum_hess/sum_grad);
+  return ((sum_hess <= T(0.0))||(sum_grad <= T(0.0))) ? -std::numeric_limits<double>::infinity() : sum_hess * std::log(sum_hess/sum_grad);
   /*
   return -(T(2.0) * sum_grad * w + (sum_hess + p.reg_lambda) * Sqr(w));
   */
 }
 
 // calculate weight given the statistics
 template <typename TrainingParams, typename T>
@@ -293,15 +293,15 @@
   return dw;
   */
 }
 
 // calculate the cost of loss function
 template <typename TrainingParams, typename T>
 XGBOOST_DEVICE inline T CalcGain(const TrainingParams &p, T sum_grad, T sum_hess) {
-  return ((sum_hess == T(0.0))||(sum_grad == T(0.0))) ? -std::numeric_limits<double>::infinity() : sum_hess*std::log(sum_hess/sum_grad);
+  return ((sum_hess <= T(0.0))||(sum_grad <= T(0.0))) ? -std::numeric_limits<double>::infinity() : sum_hess*std::log(sum_hess/sum_grad);
   /*
   if (sum_hess < p.min_child_weight) {
     return T(0.0);
   }
   if (p.max_delta_step == 0.0f) {
     if (p.reg_alpha == 0.0f) {
       return Sqr(sum_grad) / (sum_hess + p.reg_lambda);
@@ -501,16 +501,16 @@
  *
  *    "[[1, 2], [3, 4]]""
  *
  * \param p_out Pointer to output
  */
 void ParseInteractionConstraint(
     std::string const &constraint_str,
-    std::vector<std::vector<xgboost::bst_feature_t>> *p_out);
-}  // namespace xgboost
+    std::vector<std::vector<boxhed_kernel::bst_feature_t>> *p_out);
+}  // namespace boxhed_kernel
 
 // define string serializer for vector, to get the arguments
 namespace std {
 inline std::ostream &operator<<(std::ostream &os, const std::vector<int> &t) {
   os << '(';
   for (auto it = t.begin(); it != t.end(); ++it) {
     if (it != t.begin()) {
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/split_evaluator.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/split_evaluator.h`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,27 @@
  * \author Henry Gouk
  */
 
 #ifndef XGBOOST_TREE_SPLIT_EVALUATOR_H_
 #define XGBOOST_TREE_SPLIT_EVALUATOR_H_
 
 #include <dmlc/registry.h>
-#include <xgboost/base.h>
+#include <boxhed_kernel/base.h>
 #include <utility>
 #include <vector>
 #include <limits>
 
-#include "xgboost/tree_model.h"
-#include "xgboost/host_device_vector.h"
-#include "xgboost/generic_parameters.h"
+#include "boxhed_kernel/tree_model.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/generic_parameters.h"
 #include "../common/transform.h"
 #include "../common/math.h"
 #include "param.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 class TreeEvaluator {
   // hist and exact use parent id to calculate constraints.
   static constexpr bst_node_t kRootParentId =
       (-1 & static_cast<bst_node_t>((1U << 31) - 1));
 
   HostDeviceVector<float> lower_bounds_;
@@ -69,64 +69,83 @@
     common::Span<float const> upper;
     bool has_constraint;
 
     XGBOOST_DEVICE double CalcSplitGain(const ParamT &param, bst_node_t nidx,
                                         bst_feature_t fidx,
                                         tree::GradStats left,
                                         tree::GradStats right) const {
+      /*
       int constraint = constraints[fidx];
       const double negative_infinity = -std::numeric_limits<double>::infinity();
+      */
+      return this->CalcGain(nidx, param, left)+this->CalcGain(nidx, param, right);
+      /*
       double wleft = this->CalcWeight(nidx, param, left);
       double wright = this->CalcWeight(nidx, param, right);
 
       double gain = this->CalcGainGivenWeight(nidx, param, left, wleft) +
                     this->CalcGainGivenWeight(nidx, param, right, wright);
 
       if (constraint == 0) {
         return gain;
       } else if (constraint > 0) {
         return wleft <= wright ? gain : negative_infinity;
       } else {
         return wleft >= wright ? gain : negative_infinity;
       }
+      */
     }
 
     XGBOOST_DEVICE float CalcWeight(bst_node_t nodeid, const ParamT &param,
                                     tree::GradStats stats) const {
-      float w = xgboost::tree::CalcWeight(param, stats);
+      return ((stats.sum_grad == 0.0)||(stats.sum_hess == 0.0)) ? 0.0 : std::log(stats.sum_hess/stats.sum_grad);
+      /*
+      float w = boxhed_kernel::tree::CalcWeight(param, stats);
       if (!has_constraint) {
         return w;
       }
 
       if (nodeid == kRootParentId) {
         return w;
       } else if (w < lower(nodeid)) {
         return lower[nodeid];
       } else if (w > upper(nodeid)) {
         return upper[nodeid];
       } else {
         return w;
       }
+      */
     }
     XGBOOST_DEVICE float CalcGainGivenWeight(bst_node_t, ParamT const &p,
                                              tree::GradStats stats, float w) const {
+      return ((stats.sum_hess <= 0.0)||(stats.sum_grad <= 0.0)) ? 
+                      -std::numeric_limits<double>::infinity() : 
+                      stats.sum_hess*std::log(stats.sum_hess/stats.sum_grad);
+      /*                
       if (stats.GetHess() <= 0) {
         return .0f;
       }
       // Avoiding tree::CalcGainGivenWeight can significantly reduce avg floating point error.
       if (p.max_delta_step == 0.0f && has_constraint == false) {
         return Sqr(ThresholdL1(stats.sum_grad, p.reg_alpha)) /
                (stats.sum_hess + p.reg_lambda);
       }
       return tree::CalcGainGivenWeight<ParamT, float>(p, stats.sum_grad,
                                                       stats.sum_hess, w);
+      */
     }
     XGBOOST_DEVICE float CalcGain(bst_node_t nid, ParamT const &p,
                                   tree::GradStats stats) const {
+      return ((stats.sum_hess <= 0.0)||(stats.sum_grad <= 0.0)) ? 
+                      -std::numeric_limits<double>::infinity() : 
+                      stats.sum_hess*std::log(stats.sum_hess/stats.sum_grad);
+      
+      /*
       return this->CalcGainGivenWeight(nid, p, stats, this->CalcWeight(nid, p, stats));
+      */
     }
   };
 
  public:
   /* Get a view to the evaluator that can be passed down to device. */
   template <typename ParamT = TrainParam> auto GetEvaluator() const {
     if (device_ != GenericParameter::kCpuId) {
@@ -171,10 +190,10 @@
           }
         },
         common::Range(0, 1), device_, false)
         .Eval(&lower_bounds_, &upper_bounds_, &monotone_);
   }
 };
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_TREE_SPLIT_EVALUATOR_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/tree_model.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/tree_model.cc`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,29 @@
  * Copyright 2015-2020 by Contributors
  * \file tree_model.cc
  * \brief model structure for tree
  */
 #include <dmlc/registry.h>
 #include <dmlc/json.h>
 
-#include <xgboost/tree_model.h>
-#include <xgboost/logging.h>
-#include <xgboost/json.h>
+#include <boxhed_kernel/tree_model.h>
+#include <boxhed_kernel/logging.h>
+#include <boxhed_kernel/json.h>
 
 #include <sstream>
 #include <limits>
 #include <cmath>
 #include <iomanip>
 #include <stack>
 
 #include "param.h"
 #include "../common/common.h"
 #include "../common/categorical.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 // register tree parameter
 DMLC_REGISTER_PARAMETER(TreeParam);
 
 namespace tree {
 DMLC_REGISTER_PARAMETER(TrainParam);
 }
 
@@ -136,22 +136,22 @@
 };
 
 struct TreeGenReg : public dmlc::FunctionRegEntryBase<
   TreeGenReg,
   std::function<TreeGenerator* (
       FeatureMap const& fmap, std::string attrs, bool with_stats)> > {
 };
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 
 namespace dmlc {
-DMLC_REGISTRY_ENABLE(::xgboost::TreeGenReg);
+DMLC_REGISTRY_ENABLE(::boxhed_kernel::TreeGenReg);
 }  // namespace dmlc
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 TreeGenerator* TreeGenerator::Create(std::string const& attrs, FeatureMap const& fmap,
                                      bool with_stats) {
   auto pos = attrs.find(':');
   std::string name;
   std::string params;
   if (pos != std::string::npos) {
@@ -161,26 +161,26 @@
     size_t pos = std::string::npos;
     while ((pos = params.find('\'')) != std::string::npos) {
       params.replace(pos, 1, "\"");
     }
   } else {
     name = attrs;
   }
-  auto *e = ::dmlc::Registry< ::xgboost::TreeGenReg>::Get()->Find(name);
+  auto *e = ::dmlc::Registry< ::boxhed_kernel::TreeGenReg>::Get()->Find(name);
   if (e == nullptr) {
     LOG(FATAL) << "Unknown Model Builder:" << name;
   }
   auto p_io_builder = (e->body)(fmap, params, with_stats);
   return p_io_builder;
 }
 
 #define XGBOOST_REGISTER_TREE_IO(UniqueId, Name)                        \
-  static DMLC_ATTRIBUTE_UNUSED ::xgboost::TreeGenReg&                   \
+  static DMLC_ATTRIBUTE_UNUSED ::boxhed_kernel::TreeGenReg&                   \
   __make_ ## TreeGenReg ## _ ## UniqueId ## __ =                        \
-                  ::dmlc::Registry< ::xgboost::TreeGenReg>::Get()->__REGISTER__(Name)
+                  ::dmlc::Registry< ::boxhed_kernel::TreeGenReg>::Get()->__REGISTER__(Name)
 
 
 class TextGenerator : public TreeGenerator {
   using SuperT = TreeGenerator;
 
  public:
   TextGenerator(FeatureMap const& fmap, bool with_stats) :
@@ -1248,8 +1248,8 @@
   // Preallocate space for the unique path data
   const int maxd = this->MaxDepth(0) + 2;
   std::vector<PathElement> unique_path_data((maxd * (maxd + 1)) / 2);
 
   TreeShap(feat, out_contribs, 0, 0, unique_path_data.data(),
            1, 1, -1, condition, condition_feature, 1);
 }
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_basemaker-inl.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_basemaker-inl.h`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 #include <vector>
 #include <algorithm>
 #include <string>
 #include <limits>
 #include <utility>
 
-#include "xgboost/base.h"
-#include "xgboost/json.h"
-#include "xgboost/tree_updater.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/json.h"
+#include "boxhed_kernel/tree_updater.h"
 #include "param.h"
 #include "constraints.h"
 
 #include "../common/io.h"
 #include "../common/random.h"
 #include "../common/quantile.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 /*!
  * \brief base tree maker class that defines common operation
  *  needed in tree making
  */
 class BaseMaker: public TreeUpdater {
  public:
@@ -476,9 +476,9 @@
     node2workindex_.resize(tree.param.num_nodes);
     for (size_t i = 0; i < qexpand_.size(); ++i) {
       node2workindex_[qexpand_[i]] = static_cast<int>(i);
     }
   }
 };
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 #endif  // XGBOOST_TREE_UPDATER_BASEMAKER_INL_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_colmaker.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_colmaker.cc`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
  */
 #include <rabit/rabit.h>
 #include <memory>
 #include <vector>
 #include <cmath>
 #include <algorithm>
 
-#include "xgboost/parameter.h"
-#include "xgboost/tree_updater.h"
-#include "xgboost/logging.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/tree_updater.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/json.h"
 #include "param.h"
 #include "constraints.h"
 #include "../common/random.h"
 #include "split_evaluator.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 DMLC_REGISTRY_FILE_TAG(updater_colmaker);
 
 struct ColMakerTrainParam : XGBoostParameter<ColMakerTrainParam> {
   // speed optimization for dense column
   float opt_dense_col;
@@ -619,8 +619,8 @@
 
 XGBOOST_REGISTER_TREE_UPDATER(ColMaker, "grow_colmaker")
 .describe("Grow tree with parallelization over columns.")
 .set_body([]() {
     return new ColMaker();
   });
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_gpu_common.cuh` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_gpu_common.cuh`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #include <stdexcept>
 #include <string>
 #include <vector>
 #include "../common/device_helpers.cuh"
 #include "../common/random.h"
 #include "param.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 struct GPUTrainingParam {
   // minimum amount of hessian(weight) allowed in a child
   float min_child_weight;
   // L2 regularization factor
   float reg_lambda;
@@ -129,8 +129,8 @@
   XGBOOST_DEVICE T operator()(T block_aggregate) {
     T old_prefix = running_total;
     running_total += block_aggregate;
     return old_prefix;
   }
 };
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_gpu_hist.cu` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_gpu_hist.cu`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /*!
  * Copyright 2017-2020 XGBoost contributors
  */
 #include <thrust/copy.h>
 #include <thrust/reduce.h>
-#include <xgboost/tree_updater.h>
+#include <boxhed_kernel/tree_updater.h>
 #include <algorithm>
 #include <cmath>
 #include <memory>
 #include <limits>
 #include <utility>
 #include <vector>
 
-#include "xgboost/host_device_vector.h"
-#include "xgboost/parameter.h"
-#include "xgboost/span.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/host_device_vector.h"
+#include "boxhed_kernel/parameter.h"
+#include "boxhed_kernel/span.h"
+#include "boxhed_kernel/json.h"
 
 #include "../common/io.h"
 #include "../common/device_helpers.cuh"
 #include "../common/hist_util.h"
 #include "../common/bitfield.h"
 #include "../common/timer.h"
 #include "../common/categorical.h"
@@ -31,15 +31,15 @@
 #include "gpu_hist/feature_groups.cuh"
 #include "gpu_hist/gradient_based_sampler.cuh"
 #include "gpu_hist/row_partitioner.cuh"
 #include "gpu_hist/histogram.cuh"
 #include "gpu_hist/evaluate_splits.cuh"
 #include "gpu_hist/driver.cuh"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 #if !defined(GTEST_TEST)
 DMLC_REGISTRY_FILE_TAG(updater_gpu_hist);
 #endif  // !defined(GTEST_TEST)
 
 // training parameters specific to this algorithm
 struct GPUHistMakerTrainParam
@@ -328,14 +328,16 @@
         column_sampler.GetFeatureSet(tree.GetDepth(right_nidx));
     right_sampled_features->SetDevice(device_id);
     common::Span<bst_feature_t> right_feature_set =
         interaction_constraints.Query(right_sampled_features->DeviceSpan(),
                                       left_nidx);
     auto matrix = page->GetDeviceAccessor(device_id);
 
+    //std::cout<<candidate.split.left_sum.GetGrad()<<" "<<candidate.split.left_sum.GetHess()<<std::endl;
+    //std::cout<<candidate.split.right_sum.GetGrad()<<" "<<candidate.split.right_sum.GetHess()<<std::endl;
     EvaluateSplitInputs<GradientSumT> left{
       left_nidx,
       {candidate.split.left_sum.GetGrad(),
             candidate.split.left_sum.GetHess()},
           gpu_param,
           left_feature_set,
           feature_types,
@@ -564,14 +566,15 @@
   void BuildHistLeftRight(const ExpandEntry &candidate, int nidx_left,
         int nidx_right, dh::AllReducer* reducer) {
     auto build_hist_nidx = nidx_left;
     auto subtraction_trick_nidx = nidx_right;
 
     // Decide whether to build the left histogram or right histogram
     // Use sum of Hessian as a heuristic to select node with fewest training instances
+    // std::cout<<candidate.split.left_sum.GetGrad()<<" "<<candidate.split.left_sum.GetHess()<<std::endl;
     bool fewer_right = candidate.split.right_sum.GetHess() < candidate.split.left_sum.GetHess();
     if (fewer_right) {
       std::swap(build_hist_nidx, subtraction_trick_nidx);
     }
 
     this->BuildHist(build_hist_nidx);
     this->AllReduceHist(build_hist_nidx, reducer);
@@ -653,14 +656,15 @@
     this->BuildHist(kRootNIdx);
     this->AllReduceHist(kRootNIdx, reducer);
 
     // Remember root stats
     node_sum_gradients[kRootNIdx] = root_sum;
     p_tree->Stat(kRootNIdx).sum_hess = root_sum.GetHess();
     auto weight = CalcWeight(param, root_sum);
+    //std::cout<<"U:"<<root_sum.GetGrad()<<"      V:"<<root_sum.GetHess()<<"      root weight:"<<weight<<std::endl;
     p_tree->Stat(kRootNIdx).base_weight = weight;
     (*p_tree)[kRootNIdx].SetLeaf(param.learning_rate * weight);
 
     // Generate first split
     auto split = this->EvaluateRootSplit(root_sum);
     dh::TemporaryArray<ExpandEntry> entries(1);
     auto d_entries = entries.data().get();
@@ -684,41 +688,88 @@
   }
 
   void UpdateTree(HostDeviceVector<GradientPair>* gpair_all, DMatrix* p_fmat,
                   RegTree* p_tree, dh::AllReducer* reducer) {
     auto& tree = *p_tree;
     Driver driver(static_cast<TrainParam::TreeGrowPolicy>(param.grow_policy));
 
+    /*
+    const std::vector<GradientPair>& preds_h = gpair_all->HostVector();
+    auto val = preds_h[0].GetGrad();
+    int cnt = 0;
+    for (auto & gpair:preds_h){
+      std::cout << gpair.GetGrad() << ", ";
+      cnt ++;
+      if (cnt>100)
+      {
+        std::cout << std::endl;
+        break;
+      }
+      if (gpair.GetGrad()<val){
+        val = gpair.GetGrad();
+      }
+      //std::cout<<gpair.GetGrad()<<" "<<gpair.GetHess()<<std::endl;
+    }
+    std::cout<<"MIN VAL:"<<" "<< val <<std::endl;
+    */
+
+    /*
+    const std::vector<GradientPair>& preds_h = gpair_all->HostVector();
+    auto val = preds_h[0].GetGrad();
+    auto val_ = preds_h[0].GetGrad();
+    for (auto & gpair:preds_h){
+      if (gpair.GetGrad()<val){
+        val = gpair.GetGrad();
+      }
+      if (gpair.GetGrad()>val_){
+        val_ = gpair.GetGrad();
+      }
+      //std::cout<<gpair.GetGrad()<<" "<<gpair.GetHess()<<std::endl;
+    }
+    std::cout<<"MIN/MAX VAL:"<<" "<< val - val_ <<std::endl;
+    */
     monitor.Start("Reset");
     this->Reset(gpair_all, p_fmat, p_fmat->Info().num_col_);
     monitor.Stop("Reset");
 
     monitor.Start("InitRoot");
     driver.Push({ this->InitRoot(p_tree, reducer) });
     monitor.Stop("InitRoot");
 
     auto num_leaves = 1;
 
     // The set of leaves that can be expanded asynchronously
     auto expand_set = driver.Pop();
     while (!expand_set.empty()) {
+      //std::cout << "size: " << expand_set.size() << std::endl;
       auto new_candidates =
           pinned.GetSpan<ExpandEntry>(expand_set.size() * 2, ExpandEntry());
 
       for (auto i = 0ull; i < expand_set.size(); i++) {
         auto candidate = expand_set.at(i);
         if (!candidate.IsValid(param, num_leaves)) {
           continue;
         }
         this->ApplySplit(candidate, p_tree);
 
         num_leaves++;
 
         int left_child_nidx = tree[candidate.nid].LeftChild();
         int right_child_nidx = tree[candidate.nid].RightChild();
+        /*
+        if (candidate.nid == 0)
+          std::cout << "0000000000000000000000000000" << std::endl;
+        
+        std::cout << candidate.nid << std::endl;
+        //std::cout<<": " << candidate.split << std::endl;
+        //std::cout<<"    "<<  left_child_nidx  << ": " << candidate.split.left_sum.GetGrad()/val  << "          " << candidate.split.left_sum.GetGrad()  << ", " << candidate.split.left_sum.GetHess()  <<std::endl;
+        //std::cout<<"    "<<  right_child_nidx << ": " << candidate.split.right_sum.GetGrad()/val << "          " << candidate.split.right_sum.GetGrad() << ", " << candidate.split.right_sum.GetHess() <<std::endl;
+        std::cout<<"    "<<  left_child_nidx  << ": " << std::log(candidate.split.left_sum.GetGrad()  / candidate.split.left_sum.GetHess())  << "          " << candidate.split.left_sum.GetGrad()  << ", " << candidate.split.left_sum.GetHess()  <<std::endl;
+        std::cout<<"    "<<  right_child_nidx << ": " << std::log(candidate.split.right_sum.GetGrad() / candidate.split.right_sum.GetHess()) << "          " << candidate.split.right_sum.GetGrad() << ", " << candidate.split.right_sum.GetHess() <<std::endl;
+        */
         // Only create child entries if needed
         if (ExpandEntry::ChildIsValid(param, tree.GetDepth(left_child_nidx),
                                       num_leaves)) {
           monitor.Start("UpdatePosition");
           this->UpdatePosition(candidate.nid, p_tree);
           monitor.Stop("UpdatePosition");
 
@@ -770,15 +821,15 @@
     monitor_.Start("Update");
 
     // rescale learning rate according to size of trees
     float lr = param_.learning_rate;
     param_.learning_rate = lr / trees.size();
     // build tree
     try {
-      for (xgboost::RegTree* tree : trees) {
+      for (boxhed_kernel::RegTree* tree : trees) {
         this->UpdateTree(gpair, dmat, tree);
 
         if (hist_maker_param_.debug_synchronize) {
           this->CheckTreesSynchronized(tree);
         }
       }
       dh::safe_cuda(cudaGetLastError());
@@ -962,8 +1013,8 @@
 #if !defined(GTEST_TEST)
 XGBOOST_REGISTER_TREE_UPDATER(GPUHistMaker, "grow_gpu_hist")
     .describe("Grow tree with GPU.")
     .set_body([]() { return new GPUHistMaker(); });
 #endif  // !defined(GTEST_TEST)
 
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_histmaker.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_histmaker.cc`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
  * \brief use histogram counting to construct a tree
  * \author Tianqi Chen
  */
 #include <rabit/rabit.h>
 #include <vector>
 #include <algorithm>
 
-#include "xgboost/tree_updater.h"
-#include "xgboost/base.h"
-#include "xgboost/logging.h"
+#include "boxhed_kernel/tree_updater.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/logging.h"
 
 #include "../common/quantile.h"
 #include "../common/group_data.h"
 #include "./updater_basemaker-inl.h"
 #include "constraints.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 DMLC_REGISTRY_FILE_TAG(updater_histmaker);
 
 class HistMaker: public BaseMaker {
  public:
   void Update(HostDeviceVector<GradientPair> *gpair,
@@ -739,8 +739,8 @@
 // The updater for approx tree method.
 XGBOOST_REGISTER_TREE_UPDATER(HistMaker, "grow_histmaker")
 .describe("Tree constructor that uses approximate global of histogram construction.")
 .set_body([]() {
     return new GlobalProposalHistMaker();
   });
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_prune.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_prune.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 /*!
  * Copyright 2014-2020 by Contributors
  * \file updater_prune.cc
  * \brief prune a tree given the statistics
  * \author Tianqi Chen
  */
 #include <rabit/rabit.h>
-#include <xgboost/tree_updater.h>
+#include <boxhed_kernel/tree_updater.h>
 
 #include <string>
 #include <memory>
 
-#include "xgboost/base.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/base.h"
+#include "boxhed_kernel/json.h"
 #include "./param.h"
 #include "../common/io.h"
 #include "../common/timer.h"
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 DMLC_REGISTRY_FILE_TAG(updater_prune);
 
 /*! \brief pruner that prunes a tree after growing finishes */
 class TreePruner: public TreeUpdater {
  public:
@@ -113,8 +113,8 @@
 
 XGBOOST_REGISTER_TREE_UPDATER(TreePruner, "prune")
 .describe("Pruner that prune the tree according to statistics.")
 .set_body([]() {
     return new TreePruner();
   });
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_quantile_hist.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_quantile_hist.cc`

 * *Files 0% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 #include <algorithm>
 #include <queue>
 #include <iomanip>
 #include <numeric>
 #include <string>
 #include <utility>
 
-#include "xgboost/logging.h"
-#include "xgboost/tree_updater.h"
+#include "boxhed_kernel/logging.h"
+#include "boxhed_kernel/tree_updater.h"
 
 #include "constraints.h"
 #include "param.h"
 #include "./updater_quantile_hist.h"
 #include "./split_evaluator.h"
 #include "../common/random.h"
 #include "../common/hist_util.h"
 #include "../common/row_set.h"
 #include "../common/column_matrix.h"
 #include "../common/threading_utils.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 DMLC_REGISTRY_FILE_TAG(updater_quantile_hist);
 
 DMLC_REGISTER_PARAMETER(CPUHistMakerTrainParam);
 
 void QuantileHistMaker::Configure(const Args& args) {
@@ -80,15 +80,15 @@
     gmat_.Init(dmat, static_cast<uint32_t>(param_.max_bin));
     column_matrix_.Init(gmat_, param_.sparse_threshold);
     if (param_.enable_feature_grouping > 0) {
       gmatb_.Init(gmat_, column_matrix_, param_);
     }
     updater_monitor_.Stop("GmatInitialization");
     // A proper solution is puting cut matrix in DMatrix, see:
-    // https://github.com/dmlc/xgboost/issues/5143
+    // https://github.com/dmlc/boxhed_kernel/issues/5143
     is_gmat_initialized_ = true;
   }
   // rescale learning rate according to size of trees
   float lr = param_.learning_rate;
   param_.learning_rate = lr / trees.size();
   int_constraint_.Configure(param_, dmat->Info().num_col_);
   // build tree
@@ -1078,15 +1078,15 @@
                                                                  range.begin(), range.end());
   const bst_uint fid = tree[nid].SplitIndex();
   const bool default_left = tree[nid].DefaultLeft();
   const auto column_ptr = column_matrix.GetColumn<BinIdxType>(fid);
 
   std::pair<size_t, size_t> child_nodes_sizes;
 
-  if (column_ptr->GetType() == xgboost::common::kDenseColumn) {
+  if (column_ptr->GetType() == boxhed_kernel::common::kDenseColumn) {
     const common::DenseColumn<BinIdxType>& column =
           static_cast<const common::DenseColumn<BinIdxType>& >(*(column_ptr.get()));
     if (default_left) {
       if (column_matrix.AnyMissing()) {
         child_nodes_sizes = PartitionDenseKernel<true, true>(column, rid_span, split_cond,
                                                              left, right);
       } else {
@@ -1390,8 +1390,8 @@
 XGBOOST_REGISTER_TREE_UPDATER(QuantileHistMaker, "grow_quantile_histmaker")
 .describe("Grow tree using quantized histogram.")
 .set_body(
     []() {
       return new QuantileHistMaker();
     });
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_quantile_hist.h` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_quantile_hist.h`

 * *Files 3% similar despite different names*

```diff
@@ -5,36 +5,36 @@
  * \author Philip Cho, Tianqi Chen, Egor Smirnov
  */
 #ifndef XGBOOST_TREE_UPDATER_QUANTILE_HIST_H_
 #define XGBOOST_TREE_UPDATER_QUANTILE_HIST_H_
 
 #include <dmlc/timer.h>
 #include <rabit/rabit.h>
-#include <xgboost/tree_updater.h>
+#include <boxhed_kernel/tree_updater.h>
 
 #include <memory>
 #include <vector>
 #include <string>
 #include <queue>
 #include <iomanip>
 #include <unordered_map>
 #include <utility>
 
-#include "xgboost/data.h"
-#include "xgboost/json.h"
+#include "boxhed_kernel/data.h"
+#include "boxhed_kernel/json.h"
 #include "constraints.h"
 #include "./param.h"
 #include "./split_evaluator.h"
 #include "../common/random.h"
 #include "../common/timer.h"
 #include "../common/hist_util.h"
 #include "../common/row_set.h"
 #include "../common/column_matrix.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 
 /*!
  * \brief A C-style array with in-stack allocation. As long as the array is smaller than MaxStackSize, it will be allocated inside the stack. Otherwise, it will be heap-allocated.
  */
 template<typename T, size_t MaxStackSize>
 class MemStackAllocator {
  public:
@@ -64,23 +64,23 @@
   bool do_free_ = false;
   size_t required_size_;
   T stack_mem_[MaxStackSize];
 };
 
 namespace tree {
 
-using xgboost::common::GHistIndexMatrix;
-using xgboost::common::GHistIndexBlockMatrix;
-using xgboost::common::GHistIndexRow;
-using xgboost::common::HistCollection;
-using xgboost::common::RowSetCollection;
-using xgboost::common::GHistRow;
-using xgboost::common::GHistBuilder;
-using xgboost::common::ColumnMatrix;
-using xgboost::common::Column;
+using boxhed_kernel::common::GHistIndexMatrix;
+using boxhed_kernel::common::GHistIndexBlockMatrix;
+using boxhed_kernel::common::GHistIndexRow;
+using boxhed_kernel::common::HistCollection;
+using boxhed_kernel::common::RowSetCollection;
+using boxhed_kernel::common::GHistRow;
+using boxhed_kernel::common::GHistBuilder;
+using boxhed_kernel::common::ColumnMatrix;
+using boxhed_kernel::common::Column;
 
 template <typename GradientSumT>
 class HistSynchronizer;
 
 template <typename GradientSumT>
 class BatchHistSynchronizer;
 
@@ -135,15 +135,15 @@
       LOG(WARNING)
         << "Attempted to load internal configuration for a model file that was generated "
         << "by a previous version of XGBoost. A likely cause for this warning is that the model "
         << "was saved with saveRDS() in R or pickle.dump() in Python. We strongly ADVISE AGAINST "
         << "using saveRDS() or pickle.dump() so that the model remains accessible in current and "
         << "upcoming XGBoost releases. Please use xgb.save() instead to preserve models for the "
         << "long term. For more details and explanation, see "
-        << "https://xgboost.readthedocs.io/en/latest/tutorials/saving_model.html";
+        << "https://boxhed_kernel.readthedocs.io/en/latest/tutorials/saving_model.html";
       this->hist_maker_param_.UpdateAllowUnknown(Args{});
     }
   }
   void SaveConfig(Json* p_out) const override {
     auto& out = *p_out;
     out["train_param"] = ToJson(param_);
     out["cpu_hist_train_param"] = ToJson(hist_maker_param_);
@@ -196,15 +196,15 @@
   };
   // actual builder that runs the algorithm
 
   template<typename GradientSumT>
   struct Builder {
    public:
     using GHistRowT = GHistRow<GradientSumT>;
-    using GradientPairT = xgboost::detail::GradientPairInternal<GradientSumT>;
+    using GradientPairT = boxhed_kernel::detail::GradientPairInternal<GradientSumT>;
     // constructor
     explicit Builder(const TrainParam& param,
                      std::unique_ptr<TreeUpdater> pruner,
                      FeatureInteractionConstraintHost int_constraints_,
                      DMatrix const* fmat)
       : param_(param),
         tree_evaluator_(param, fmat->Info().num_col_, GenericParameter::kCpuId),
@@ -532,10 +532,10 @@
   using BuilderT = QuantileHistMaker::Builder<GradientSumT>;
   void AddHistRows(BuilderT*, int *starting_index,
                    int *sync_count, RegTree *p_tree) override;
 };
 
 
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
 
 #endif  // XGBOOST_TREE_UPDATER_QUANTILE_HIST_H_
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_refresh.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_refresh.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /*!
  * Copyright 2014 by Contributors
  * \file updater_refresh.cc
  * \brief refresh the statistics and leaf value on the tree on the dataset
  * \author Tianqi Chen
  */
 #include <rabit/rabit.h>
-#include <xgboost/tree_updater.h>
+#include <boxhed_kernel/tree_updater.h>
 
 #include <vector>
 #include <limits>
 
-#include "xgboost/json.h"
+#include "boxhed_kernel/json.h"
 #include "./param.h"
 #include "../common/io.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 DMLC_REGISTRY_FILE_TAG(updater_refresh);
 
 /*! \brief pruner that prunes a tree after growing finishs */
 class TreeRefresher: public TreeUpdater {
  public:
@@ -134,17 +134,17 @@
     tree.Stat(nid).sum_hess = static_cast<bst_float>(gstats[nid].sum_hess);
     if (tree[nid].IsLeaf()) {
       if (param_.refresh_leaf) {
         tree[nid].SetLeaf(tree.Stat(nid).base_weight * param_.learning_rate);
       }
     } else {
       tree.Stat(nid).loss_chg = static_cast<bst_float>(
-          xgboost::tree::CalcGain(param_, gstats[tree[nid].LeftChild()]) +
-          xgboost::tree::CalcGain(param_, gstats[tree[nid].RightChild()]) -
-          xgboost::tree::CalcGain(param_, gstats[nid]));
+          boxhed_kernel::tree::CalcGain(param_, gstats[tree[nid].LeftChild()]) +
+          boxhed_kernel::tree::CalcGain(param_, gstats[tree[nid].RightChild()]) -
+          boxhed_kernel::tree::CalcGain(param_, gstats[nid]));
       this->Refresh(gstats, tree[nid].LeftChild(), p_tree);
       this->Refresh(gstats, tree[nid].RightChild(), p_tree);
     }
   }
   // training parameter
   TrainParam param_;
   // reducer
@@ -153,8 +153,8 @@
 
 XGBOOST_REGISTER_TREE_UPDATER(TreeRefresher, "refresh")
 .describe("Refresher that refreshes the weight and statistics according to data.")
 .set_body([]() {
     return new TreeRefresher();
   });
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel/src/tree/updater_sync.cc` & `boxhed_kernel-2.0.2/boxhed_kernel/src/tree/updater_sync.cc`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /*!
  * Copyright 2014-2019 by Contributors
  * \file updater_sync.cc
  * \brief synchronize the tree in all distributed nodes
  */
-#include <xgboost/tree_updater.h>
+#include <boxhed_kernel/tree_updater.h>
 #include <vector>
 #include <string>
 #include <limits>
 
-#include "xgboost/json.h"
+#include "boxhed_kernel/json.h"
 #include "../common/io.h"
 
-namespace xgboost {
+namespace boxhed_kernel {
 namespace tree {
 
 DMLC_REGISTRY_FILE_TAG(updater_sync);
 
 /*!
  * \brief syncher that synchronize the tree in all distributed nodes
  * can implement various strategies, so far it is always set to node 0's tree
@@ -53,8 +53,8 @@
 
 XGBOOST_REGISTER_TREE_UPDATER(TreeSyncher, "sync")
 .describe("Syncher that synchronize the tree in all distributed nodes.")
 .set_body([]() {
     return new TreeSyncher();
   });
 }  // namespace tree
-}  // namespace xgboost
+}  // namespace boxhed_kernel
```

### Comparing `boxhed_kernel-2.0.1/boxhed_kernel.egg-info/SOURCES.txt` & `boxhed_kernel-2.0.2/boxhed_kernel.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 boxhed_kernel/CMakeLists.txt
 boxhed_kernel/LICENSE
+boxhed_kernel/VERSION
+boxhed_kernel/__init__.py
+boxhed_kernel/callback.py
+boxhed_kernel/compat.py
+boxhed_kernel/core.py
+boxhed_kernel/dask.py
+boxhed_kernel/data.py
+boxhed_kernel/libpath.py
+boxhed_kernel/plotting.py
+boxhed_kernel/rabit.py
+boxhed_kernel/sklearn.py
+boxhed_kernel/tracker.py
+boxhed_kernel/training.py
 boxhed_kernel.egg-info/PKG-INFO
 boxhed_kernel.egg-info/SOURCES.txt
 boxhed_kernel.egg-info/dependency_links.txt
 boxhed_kernel.egg-info/not-zip-safe
 boxhed_kernel.egg-info/requires.txt
 boxhed_kernel.egg-info/top_level.txt
 boxhed_kernel/cmake/Doc.cmake
 boxhed_kernel/cmake/FindPrefetchIntrinsics.cmake
 boxhed_kernel/cmake/Python_version.in
 boxhed_kernel/cmake/RPackageInstall.cmake.in
 boxhed_kernel/cmake/RPackageInstallTargetSetup.cmake
 boxhed_kernel/cmake/Sanitizer.cmake
 boxhed_kernel/cmake/Utils.cmake
 boxhed_kernel/cmake/Version.cmake
+boxhed_kernel/cmake/boxhed_kernel-config.cmake.in
+boxhed_kernel/cmake/boxhed_kernel.pc.in
 boxhed_kernel/cmake/version_config.h.in
-boxhed_kernel/cmake/xgboost-config.cmake.in
-boxhed_kernel/cmake/xgboost.pc.in
 boxhed_kernel/cmake/modules/FindASan.cmake
 boxhed_kernel/cmake/modules/FindLSan.cmake
 boxhed_kernel/cmake/modules/FindLibR.cmake
 boxhed_kernel/cmake/modules/FindNVML.cmake
 boxhed_kernel/cmake/modules/FindNVTX.cmake
 boxhed_kernel/cmake/modules/FindNccl.cmake
 boxhed_kernel/cmake/modules/FindTSan.cmake
@@ -195,36 +208,36 @@
 boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/ApplicationMaster.java
 boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/Client.java
 boxhed_kernel/dmlc-core/tracker/yarn/src/main/java/org/apache/hadoop/yarn/dmlc/TaskRecord.java
 boxhed_kernel/dmlc-core/windows/.gitignore
 boxhed_kernel/dmlc-core/windows/README.md
 boxhed_kernel/dmlc-core/windows/dmlc.sln
 boxhed_kernel/dmlc-core/windows/dmlc/dmlc.vcxproj
-boxhed_kernel/include/xgboost/base.h
-boxhed_kernel/include/xgboost/c_api.h
-boxhed_kernel/include/xgboost/data.h
-boxhed_kernel/include/xgboost/feature_map.h
-boxhed_kernel/include/xgboost/gbm.h
-boxhed_kernel/include/xgboost/generic_parameters.h
-boxhed_kernel/include/xgboost/host_device_vector.h
-boxhed_kernel/include/xgboost/intrusive_ptr.h
-boxhed_kernel/include/xgboost/json.h
-boxhed_kernel/include/xgboost/json_io.h
-boxhed_kernel/include/xgboost/learner.h
-boxhed_kernel/include/xgboost/linear_updater.h
-boxhed_kernel/include/xgboost/logging.h
-boxhed_kernel/include/xgboost/metric.h
-boxhed_kernel/include/xgboost/model.h
-boxhed_kernel/include/xgboost/objective.h
-boxhed_kernel/include/xgboost/parameter.h
-boxhed_kernel/include/xgboost/predictor.h
-boxhed_kernel/include/xgboost/span.h
-boxhed_kernel/include/xgboost/tree_model.h
-boxhed_kernel/include/xgboost/tree_updater.h
-boxhed_kernel/include/xgboost/version_config.h
+boxhed_kernel/include/boxhed_kernel/base.h
+boxhed_kernel/include/boxhed_kernel/c_api.h
+boxhed_kernel/include/boxhed_kernel/data.h
+boxhed_kernel/include/boxhed_kernel/feature_map.h
+boxhed_kernel/include/boxhed_kernel/gbm.h
+boxhed_kernel/include/boxhed_kernel/generic_parameters.h
+boxhed_kernel/include/boxhed_kernel/host_device_vector.h
+boxhed_kernel/include/boxhed_kernel/intrusive_ptr.h
+boxhed_kernel/include/boxhed_kernel/json.h
+boxhed_kernel/include/boxhed_kernel/json_io.h
+boxhed_kernel/include/boxhed_kernel/learner.h
+boxhed_kernel/include/boxhed_kernel/linear_updater.h
+boxhed_kernel/include/boxhed_kernel/logging.h
+boxhed_kernel/include/boxhed_kernel/metric.h
+boxhed_kernel/include/boxhed_kernel/model.h
+boxhed_kernel/include/boxhed_kernel/objective.h
+boxhed_kernel/include/boxhed_kernel/parameter.h
+boxhed_kernel/include/boxhed_kernel/predictor.h
+boxhed_kernel/include/boxhed_kernel/span.h
+boxhed_kernel/include/boxhed_kernel/tree_model.h
+boxhed_kernel/include/boxhed_kernel/tree_updater.h
+boxhed_kernel/include/boxhed_kernel/version_config.h
 boxhed_kernel/plugin/CMakeLists.txt
 boxhed_kernel/plugin/README.md
 boxhed_kernel/plugin/dense_parser/dense_libsvm.cc
 boxhed_kernel/plugin/example/README.md
 boxhed_kernel/plugin/example/custom_obj.cc
 boxhed_kernel/plugin/lz4/sparse_page_lz4_format.cc
 boxhed_kernel/plugin/updater_gpu/README.md
@@ -410,21 +423,8 @@
 boxhed_kernel/src/tree/gpu_hist/feature_groups.cu
 boxhed_kernel/src/tree/gpu_hist/feature_groups.cuh
 boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cu
 boxhed_kernel/src/tree/gpu_hist/gradient_based_sampler.cuh
 boxhed_kernel/src/tree/gpu_hist/histogram.cu
 boxhed_kernel/src/tree/gpu_hist/histogram.cuh
 boxhed_kernel/src/tree/gpu_hist/row_partitioner.cu
-boxhed_kernel/src/tree/gpu_hist/row_partitioner.cuh
-xgboost/VERSION
-xgboost/__init__.py
-xgboost/callback.py
-xgboost/compat.py
-xgboost/core.py
-xgboost/dask.py
-xgboost/data.py
-xgboost/libpath.py
-xgboost/plotting.py
-xgboost/rabit.py
-xgboost/sklearn.py
-xgboost/tracker.py
-xgboost/training.py
+boxhed_kernel/src/tree/gpu_hist/row_partitioner.cuh
```

### Comparing `boxhed_kernel-2.0.1/setup.py` & `boxhed_kernel-2.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Setup xgboost package."""
+"""Setup boxhed_kernel package."""
 import os
 import shutil
 import subprocess
 import logging
 import distutils
 import sys
 from platform import system
@@ -13,42 +13,40 @@
 # directory, parent directory is no longer reachable (isolated build) .
 CURRENT_DIR = os.path.abspath(os.path.dirname(__file__))
 sys.path.insert(0, CURRENT_DIR)
 
 # Options only effect `python setup.py install`, building `bdist_wheel`
 # requires using CMake directly.
 USER_OPTIONS = {
-    # libxgboost options.
+    # libboxhed_kernel options.
     'use-openmp': (None, 'Build with OpenMP support.', 1),
     'use-cuda':   (None, 'Build with GPU acceleration.', 0),
     'use-nccl':   (None, 'Build with NCCL to enable distributed GPU support.', 0),
     'build-with-shared-nccl': (None, 'Build with shared NCCL library.', 0),
     'hide-cxx-symbols':       (None, 'Hide all C++ symbols during build.', 1),
     'use-hdfs':   (None, 'Build with HDFS support', 0),
     'use-azure':  (None, 'Build with AZURE support.', 0),
     'use-s3':     (None, 'Build with S3 support', 0),
     'plugin-lz4': (None, 'Build lz4 plugin.', 0),
-    'plugin-dense-parser': (None, 'Build dense parser plugin.', 0),
-    # Python specific
-    'use-system-libxgboost': (None, 'Use libxgboost.so in system path.', 0)
+    'plugin-dense-parser': (None, 'Build dense parser plugin.', 0)
 }
 
 NEED_CLEAN_TREE = set()
 NEED_CLEAN_FILE = set()
 BUILD_TEMP_DIR = None
 
 
 def lib_name():
     '''Return platform dependent shared object name.'''
     if system() == 'Linux' or system().upper().endswith('BSD'):
-        name = 'libxgboost.so'
+        name = 'libboxhed_kernel.so'
     elif system() == 'Darwin':
-        name = 'libxgboost.dylib'
+        name = 'libboxhed_kernel.dylib'
     elif system() == 'Windows':
-        name = 'xgboost.dll'
+        name = 'boxhed_kernel.dll'
     return name
 
 
 def copy_tree(src_dir, target_dir):
     '''Copy source tree into build directory.'''
     def clean_copy_tree(src, dst):
         distutils.dir_util.copy_tree(src, dst)
@@ -120,35 +118,32 @@
                                   cwd=build_dir)
         else:
             subprocess.check_call(['cmake', '--build', '.',
                                    '--config', 'Release'], cwd=build_dir)
 
     def build_cmake_extension(self):
         '''Configure and build using CMake'''
-        if USER_OPTIONS['use-system-libxgboost'][2]:
-            self.logger.info('Using system libxgboost.')
-            return
 
         src_dir = 'boxhed_kernel'
         try:
             copy_tree(os.path.join(CURRENT_DIR, os.path.pardir),
                       os.path.join(self.build_temp, src_dir))
         except Exception:  # pylint: disable=broad-except
             copy_tree(src_dir, os.path.join(self.build_temp, src_dir))
         build_dir = self.build_temp
         global BUILD_TEMP_DIR  # pylint: disable=global-statement
         BUILD_TEMP_DIR = build_dir
-        libxgboost = os.path.abspath(
+        libboxhed_kernel = os.path.abspath(
             os.path.join(CURRENT_DIR, os.path.pardir, 'lib', lib_name()))
 
-        if os.path.exists(libxgboost):
+        if os.path.exists(libboxhed_kernel):
             self.logger.info('Found shared library, skipping build.')
             return
 
-        self.logger.info('Building from source. %s', libxgboost)
+        self.logger.info('Building from source. %s', libboxhed_kernel)
         if not os.path.exists(build_dir):
             os.mkdir(build_dir)
         if shutil.which('ninja'):
             build_tool = 'ninja'
         else:
             build_tool = 'make'
 
@@ -189,61 +184,54 @@
                 os.path.join(CURRENT_DIR, os.path.pardir, 'lib', lib_name())):
             raise ValueError('For using editable installation, please ' +
                              'build the shared object first with CMake.')
 
 
 class Sdist(sdist.sdist):       # pylint: disable=too-many-ancestors
     '''Copy c++ source into Python directory.'''
-    logger = logging.getLogger('xgboost sdist')
+    logger = logging.getLogger('boxhed_kernel sdist')
 
     def run(self):
         copy_tree(os.path.join(CURRENT_DIR, os.path.pardir),
                   os.path.join(CURRENT_DIR, 'boxhed_kernel'))
-        libxgboost = os.path.join(
+        libboxhed_kernel = os.path.join(
             CURRENT_DIR, os.path.pardir, 'lib', lib_name())
-        if os.path.exists(libxgboost):
+        if os.path.exists(libboxhed_kernel):
             self.logger.warning(
                 'Found shared library, removing to avoid being included in source distribution.'
             )
-            os.remove(libxgboost)
+            os.remove(libboxhed_kernel)
         super().run()
 
 
 class InstallLib(install_lib.install_lib):
     '''Copy shared object into installation directory.'''
-    logger = logging.getLogger('xgboost install_lib')
+    logger = logging.getLogger('boxhed_kernel install_lib')
 
     def install(self):
         outfiles = super().install()
 
-        if USER_OPTIONS['use-system-libxgboost'][2] != 0:
-            self.logger.info('Using system libxgboost.')
-            lib_path = os.path.join(sys.prefix, 'lib')
-            msg = 'use-system-libxgboost is specified, but ' + lib_name() + \
-                ' is not found in: ' + lib_path
-            assert os.path.exists(os.path.join(lib_path, lib_name())), msg
-            return []
 
         lib_dir = os.path.join(self.install_dir, 'boxhed_kernel', 'lib')
         if not os.path.exists(lib_dir):
             os.mkdir(lib_dir)
         dst = os.path.join(self.install_dir, 'boxhed_kernel', 'lib', lib_name())
 
         global BUILD_TEMP_DIR   # pylint: disable=global-statement
-        libxgboost_path = lib_name()
+        libboxhed_kernel_path = lib_name()
 
         dft_lib_dir = os.path.join(CURRENT_DIR, os.path.pardir, 'lib')
         build_dir = os.path.join(BUILD_TEMP_DIR, 'boxhed_kernel', 'lib')
 
-        if os.path.exists(os.path.join(dft_lib_dir, libxgboost_path)):
+        if os.path.exists(os.path.join(dft_lib_dir, libboxhed_kernel_path)):
             # The library is built by CMake directly
-            src = os.path.join(dft_lib_dir, libxgboost_path)
+            src = os.path.join(dft_lib_dir, libboxhed_kernel_path)
         else:
             # The library is built by setup.py
-            src = os.path.join(build_dir, libxgboost_path)
+            src = os.path.join(build_dir, libboxhed_kernel_path)
         self.logger.info('Installing shared library: %s', src)
         dst, _ = self.copy_file(src, dst)
         outfiles.append(dst)
         return outfiles
 
 
 class Install(install.install):  # pylint: disable=too-many-instance-attributes
@@ -265,15 +253,15 @@
         self.use_hdfs = 0
         self.use_azure = 0
         self.use_s3 = 0
 
         self.plugin_lz4 = 0
         self.plugin_dense_parser = 0
 
-        self.use_system_libxgboost = 0
+        self.use_system_libboxhed_kernel = 0
 
     def run(self):
         # setuptools will configure the options according to user supplied command line
         # arguments, then here we propagate them into `USER_OPTIONS` for visibility to
         # other sub-commands like `build_ext`.
         for k, v in USER_OPTIONS.items():
             arg = k.replace('-', '_')
@@ -281,39 +269,39 @@
                 USER_OPTIONS[k] = (v[0], v[1], getattr(self, arg))
         super().run()
 
 
 if __name__ == '__main__':
     # Supported commands:
     # From internet:
-    # - pip install xgboost
-    # - pip install --no-binary :all: xgboost
+    # - pip install boxhed_kernel
+    # - pip install --no-binary :all: boxhed_kernel
 
-    # From source tree `xgboost/python-package`:
+    # From source tree `boxhed_kernel/python-package`:
     # - python setup.py build
     # - python setup.py build_ext
     # - python setup.py install
     # - python setup.py sdist       && pip install <sdist-name>
     # - python setup.py bdist_wheel && pip install <wheel-name>
 
     # When XGBoost is compiled directly with CMake:
     # - pip install . -e
     # - python setup.py develop   # same as above
     logging.basicConfig(level=logging.INFO)
     setup(name='boxhed_kernel',
-          version="2.0.1",#open(os.path.join(
-          #    CURRENT_DIR, 'xgboost/VERSION')).read().strip(),
+          version="2.0.2",#open(os.path.join(
+          #    CURRENT_DIR, 'boxhed_kernel/VERSION')).read().strip(),
           description="XGBoost Python Package",
           long_description=open(os.path.join(CURRENT_DIR, 'README.rst'),
                                 encoding='utf-8').read(),
           install_requires=[
               'numpy',
               'scipy',
           ],
-          ext_modules=[CMakeExtension('libxgboost')],
+          ext_modules=[CMakeExtension('libboxhed_kernel')],
           cmdclass={
               'build_ext': BuildExt,
               'sdist': Sdist,
               'install_lib': InstallLib,
               'install': Install
           },
           extras_require={
@@ -334,10 +322,10 @@
                        'Operating System :: OS Independent',
                        'Programming Language :: Python',
                        'Programming Language :: Python :: 3',
                        'Programming Language :: Python :: 3.6',
                        'Programming Language :: Python :: 3.7',
                        'Programming Language :: Python :: 3.8'],
           python_requires='>=3.6',
-          url='https://github.com/dmlc/xgboost')
+          url='https://github.com/dmlc/boxhed_kernel')
 
     clean_up()
```

### Comparing `boxhed_kernel-2.0.1/xgboost/__init__.py` & `boxhed_kernel-2.0.2/boxhed_kernel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 """XGBoost: eXtreme Gradient Boosting library.
 
-Contributors: https://github.com/dmlc/xgboost/blob/master/CONTRIBUTORS.md
+Contributors: https://github.com/dmlc/boxhed_kernel/blob/master/CONTRIBUTORS.md
 """
 
 import os
 
 from .core import DMatrix, DeviceQuantileDMatrix, Booster
 from .training import train, cv
 from . import rabit  # noqa
```

### Comparing `boxhed_kernel-2.0.1/xgboost/callback.py` & `boxhed_kernel-2.0.2/boxhed_kernel/callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
     '''
     world = rabit.get_world_size()
     assert world != 0
     if world == 1:
         return score
     if isinstance(score, tuple):  # has mean and stdv
         raise ValueError(
-            'xgboost.cv function should not be used in distributed environment.')
+            'boxhed_kernel.cv function should not be used in distributed environment.')
     score = numpy.array([score])
     score = rabit.allreduce(score, rabit.Op.SUM) / world
     return score[0]
 
 
 class CallbackContainer:
     '''A special callback for invoking a list of other callbacks.
```

### Comparing `boxhed_kernel-2.0.1/xgboost/compat.py` & `boxhed_kernel-2.0.2/boxhed_kernel/compat.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/xgboost/core.py` & `boxhed_kernel-2.0.2/boxhed_kernel/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 import numpy as np
 import scipy.sparse
 
 from .compat import (STRING_TYPES, DataFrame, py_str, PANDAS_INSTALLED,
                      lazy_isinstance)
 from .libpath import find_lib_path
 
-# c_bst_ulong corresponds to bst_ulong defined in xgboost/c_api.h
+# c_bst_ulong corresponds to bst_ulong defined in boxhed_kernel/c_api.h
 c_bst_ulong = ctypes.c_uint64
 
 
 class XGBoostError(ValueError):
-    """Error thrown by xgboost trainer."""
+    """Error thrown by boxhed_kernel trainer."""
 
 
 class EarlyStopException(Exception):
     """Exception to signal early stopping.
 
     Parameters
     ----------
@@ -124,15 +124,15 @@
     """Wrap log_callback() method in ctypes callback type"""
     # pylint: disable=invalid-name
     CALLBACK = ctypes.CFUNCTYPE(None, ctypes.c_char_p)
     return CALLBACK(_log_callback)
 
 
 def _load_lib():
-    """Load xgboost Library."""
+    """Load boxhed_kernel Library."""
     lib_paths = find_lib_path()
     if not lib_paths:
         return None
     try:
         pathBackup = os.environ['PATH'].split(os.pathsep)
     except KeyError:
         pathBackup = []
@@ -357,15 +357,15 @@
         '''Set the next batch of data.
 
         Parameters
         ----------
 
         data_handle: callable
             A function with same data fields like `data`, `label` with
-            `xgboost.DMatrix`.
+            `boxhed_kernel.DMatrix`.
 
         Returns
         -------
         0 if there's no more batch, otherwise 1.
 
         '''
         raise NotImplementedError()
@@ -441,15 +441,15 @@
         """Parameters
         ----------
         data : os.PathLike/string/numpy.array/scipy.sparse/pd.DataFrame/
                dt.Frame/cudf.DataFrame/cupy.array/dlpack
             Data source of DMatrix.
             When data is string or os.PathLike type, it represents the path
             libsvm format txt file, csv file (by specifying uri parameter
-            'path_to_csv?format=csv'), or binary file that xgboost can read
+            'path_to_csv?format=csv'), or binary file that boxhed_kernel can read
             from.
         label : list, numpy 1-D array or cudf.DataFrame, optional
             Label of the training data.
         missing : float, optional
             Value in the input data which needs to be present as a missing
             value. If None, defaults to np.nan.
         weight : list, numpy 1-D array or cudf.DataFrame , optional
@@ -629,15 +629,15 @@
             The array of data to be set
         """
         from .data import dispatch_meta_backend
         dispatch_meta_backend(self, data, field, 'uint32')
 
     def save_binary(self, fname, silent=True):
         """Save DMatrix to an XGBoost buffer.  Saved binary can be later loaded
-        by providing the path to :py:func:`xgboost.DMatrix` as input.
+        by providing the path to :py:func:`boxhed_kernel.DMatrix` as input.
 
         Parameters
         ----------
         fname : string or os.PathLike
             Name of the output buffer file.
         silent : bool (optional; default: True)
             If set, the output is suppressed.
@@ -980,15 +980,15 @@
         )
 
 
 class Booster(object):
     # pylint: disable=too-many-public-methods
     """A Booster of XGBoost.
 
-    Booster is the model of xgboost, that contains low level routines for
+    Booster is the model of boxhed_kernel, that contains low level routines for
     training, prediction and evaluation.
     """
 
     feature_names = None
 
     def __init__(self, params=None, cache=(), model_file=None):
         # pylint: disable=invalid-name
@@ -1270,15 +1270,15 @@
         else:
             pred = self.predict(dtrain, output_margin=True, training=True)
             grad, hess = fobj(pred, dtrain)
             self.boost(dtrain, grad, hess)
 
     def boost(self, dtrain, grad, hess):
         """Boost the booster for one iteration, with customized gradient
-        statistics.  Like :func:`xgboost.core.Booster.update`, this
+        statistics.  Like :func:`boxhed_kernel.core.Booster.update`, this
         function should not be called directly by users.
 
         Parameters
         ----------
         dtrain : DMatrix
             The training DMatrix.
         grad : list
@@ -1657,15 +1657,15 @@
     def save_model(self, fname):
         """Save the model to a file.
 
         The model is saved in an XGBoost internal format which is universal
         among the various XGBoost interfaces. Auxiliary attributes of the
         Python Booster object (such as feature_names) will not be saved.  See:
 
-          https://xgboost.readthedocs.io/en/latest/tutorials/saving_model.html
+          https://boxhed_kernel.readthedocs.io/en/latest/tutorials/saving_model.html
 
         for more info.
 
         Parameters
         ----------
         fname : string or os.PathLike
             Output file name
@@ -1695,15 +1695,15 @@
         """Load the model from a file or bytearray. Path to file can be local
         or as an URI.
 
         The model is loaded from XGBoost format which is universal among the
         various XGBoost interfaces. Auxiliary attributes of the Python Booster
         object (such as feature_names) will not be loaded.  See:
 
-          https://xgboost.readthedocs.io/en/latest/tutorials/saving_model.html
+          https://boxhed_kernel.readthedocs.io/en/latest/tutorials/saving_model.html
 
         for more info.
 
         Parameters
         ----------
         fname : string, os.PathLike, or a memory buffer
             Input file name or memory buffer(see also save_raw)
```

### Comparing `boxhed_kernel-2.0.1/xgboost/dask.py` & `boxhed_kernel-2.0.2/boxhed_kernel/dask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # pylint: disable=too-many-arguments, too-many-locals
 # pylint: disable=missing-class-docstring, invalid-name
 # pylint: disable=too-many-lines
 """Dask extensions for distributed training. See
-https://xgboost.readthedocs.io/en/latest/tutorials/dask.html for simple
-tutorial.  Also xgboost/demo/dask for some examples.
+https://boxhed_kernel.readthedocs.io/en/latest/tutorials/dask.html for simple
+tutorial.  Also boxhed_kernel/demo/dask for some examples.
 
 There are two sets of APIs in this module, one is the functional API including
 ``train`` and ``predict`` methods.  Another is stateful Scikit-Learner wrapper
 inherited from single-node Scikit-Learn interface.
 
-The implementation is heavily influenced by dask_xgboost:
-https://github.com/dask/dask-xgboost
+The implementation is heavily influenced by dask_boxhed_kernel:
+https://github.com/dask/dask-boxhed_kernel
 
 """
 import platform
 import logging
 from collections import defaultdict
 from collections.abc import Sequence
 from threading import Thread
@@ -31,15 +31,15 @@
 from .compat import lazy_isinstance
 
 from .core import DMatrix, DeviceQuantileDMatrix, Booster, _expect, DataIter
 from .core import _deprecate_positional_args
 from .training import train as worker_train
 from .tracker import RabitTracker
 from .sklearn import XGBModel, XGBRegressorBase, XGBClassifierBase
-from .sklearn import xgboost_model_doc
+from .sklearn import boxhed_kernel_model_doc
 
 
 dd = LazyLoader('dd', globals(), 'dask.dataframe')
 da = LazyLoader('da', globals(), 'dask.array')
 dask = LazyLoader('dask', globals(), 'dask')
 distributed = LazyLoader('distributed', globals(), 'dask.distributed')
 
@@ -60,15 +60,15 @@
 #   for the implementation here:
 #     - Synchronous world is different from asynchronous one, and they don't
 #       mix well.
 #     - Write everything with async, then use distributed Client sync function
 #       to do the switch.
 
 
-LOGGER = logging.getLogger('[xgboost.dask]')
+LOGGER = logging.getLogger('[boxhed_kernel.dask]')
 
 
 def _start_tracker(n_workers):
     """Start Rabit tracker """
     env = {'DMLC_NUM_WORKER': n_workers}
     import socket
     host = socket.gethostbyname(socket.gethostname())
@@ -86,26 +86,26 @@
     try:
         import dask             # pylint: disable=W0621,W0611
     except ImportError as e:
         raise ImportError(
             'Dask needs to be installed in order to use this module') from e
 
     if platform.system() == 'Windows':
-        msg = 'Windows is not officially supported for dask/xgboost,'
+        msg = 'Windows is not officially supported for dask/boxhed_kernel,'
         msg += ' contribution are welcomed.'
         LOGGER.warning(msg)
 
 
 class RabitContext:
     '''A context controling rabit initialization and finalization.'''
     def __init__(self, args):
         self.args = args
         worker = distributed.get_worker()
         self.args.append(
-            ('DMLC_TASK_ID=[xgboost.dask]:' + str(worker.address)).encode())
+            ('DMLC_TASK_ID=[boxhed_kernel.dask]:' + str(worker.address)).encode())
 
     def __enter__(self):
         rabit.init(self.args)
         LOGGER.debug('-------------- rabit say hello ------------------')
 
     def __exit__(self, *args):
         rabit.finalize()
@@ -256,15 +256,15 @@
                 ' chunks=(partition_size, X.shape[1])'
 
         data = data.persist()
         for meta in [label, weights, base_margin, label_lower_bound,
                      label_upper_bound]:
             if meta is not None:
                 meta = meta.persist()
-        # Breaking data into partitions, a trick borrowed from dask_xgboost.
+        # Breaking data into partitions, a trick borrowed from dask_boxhed_kernel.
 
         # `to_delayed` downgrades high-level objects into numpy or pandas
         # equivalents.
         X_parts = data.to_delayed()
         if isinstance(X_parts, numpy.ndarray):
             check_columns(X_parts)
             X_parts = X_parts.flatten().tolist()
@@ -353,15 +353,15 @@
     for i, _ in enumerate(list_of_parts):
         data = list_of_parts[i][0]
         labels = None
         weights = None
         base_margin = None
         label_lower_bound = None
         label_upper_bound = None
-        # Iterate through all possible meta info, brings small overhead as in xgboost
+        # Iterate through all possible meta info, brings small overhead as in boxhed_kernel
         # there are constant number of meta info available.
         for j, blob in enumerate(list_of_parts[i][1:]):
             if meta_names[j] == 'labels':
                 labels = blob
             elif meta_names[j] == 'weights':
                 weights = blob
             elif meta_names[j] == 'base_margin':
@@ -716,27 +716,27 @@
 
     Parameters
     ----------
     client: dask.distributed.Client
         Specify the dask client used for training.  Use default client
         returned from dask if it's set to None.
     \\*\\*kwargs:
-        Other parameters are the same as `xgboost.train` except for
+        Other parameters are the same as `boxhed_kernel.train` except for
         `evals_result`, which is returned as part of function return value
         instead of argument.
 
     Returns
     -------
     results: dict
         A dictionary containing trained booster and evaluation history.
-        `history` field is the same as `eval_result` from `xgboost.train`.
+        `history` field is the same as `eval_result` from `boxhed_kernel.train`.
 
         .. code-block:: python
 
-            {'booster': xgboost.Booster,
+            {'booster': boxhed_kernel.Booster,
              'history': {'train': {'logloss': ['0.48253', '0.35953']},
                          'eval': {'logloss': ['0.480385', '0.357756']}}}
 
     '''
     _assert_dask_support()
     client = _xgb_get_client(client)
     return client.sync(
@@ -894,15 +894,15 @@
     .. versionadded:: 1.0.0
 
     Parameters
     ----------
     client: dask.distributed.Client
         Specify the dask client used for training.  Use default client
         returned from dask if it's set to None.
-    model: A Booster or a dictionary returned by `xgboost.dask.train`.
+    model: A Booster or a dictionary returned by `boxhed_kernel.dask.train`.
         The trained model.
     data: DaskDMatrix/dask.dataframe.DataFrame/dask.array.Array
         Input data used for prediction.  When input is a dataframe object,
         prediction output is a series.
     missing: float
         Used when input data is not DaskDMatrix.  Specify the value
         considered as missing.
@@ -1082,15 +1082,15 @@
         return client
 
     @client.setter
     def client(self, clt):
         self._client = clt
 
 
-@xgboost_model_doc("""Implementation of the Scikit-Learn API for XGBoost.""",
+@boxhed_kernel_model_doc("""Implementation of the Scikit-Learn API for XGBoost.""",
                    ['estimators', 'model'])
 class DaskXGBRegressor(DaskScikitLearnBase, XGBRegressorBase):
     # pylint: disable=missing-class-docstring
     async def _fit_async(self, X, y, sample_weight, base_margin, eval_set,
                          sample_weight_eval_set, early_stopping_rounds,
                          verbose):
         dtrain = await DaskDMatrix(client=self.client,
@@ -1153,15 +1153,15 @@
     def predict(self, data, output_margin=False, base_margin=None):
         _assert_dask_support()
         return self.client.sync(self._predict_async, data,
                                 output_margin=output_margin,
                                 base_margin=base_margin)
 
 
-@xgboost_model_doc(
+@boxhed_kernel_model_doc(
     'Implementation of the scikit-learn API for XGBoost classification.',
     ['estimators', 'model'])
 class DaskXGBClassifier(DaskScikitLearnBase, XGBClassifierBase):
     # pylint: disable=missing-class-docstring
     async def _fit_async(self, X, y, sample_weight, base_margin, eval_set,
                          sample_weight_eval_set, early_stopping_rounds,
                          verbose):
```

### Comparing `boxhed_kernel-2.0.1/xgboost/data.py` & `boxhed_kernel-2.0.2/boxhed_kernel/data.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/xgboost/libpath.py` & `boxhed_kernel-2.0.2/boxhed_kernel/libpath.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # coding: utf-8
-"""Find the path to xgboost dynamic library files."""
+"""Find the path to boxhed_kernel dynamic library files."""
 
 import os
 import platform
 import sys
 
 
 class XGBoostLibraryNotFound(Exception):
-    """Error thrown by when xgboost is not found"""
+    """Error thrown by when boxhed_kernel is not found"""
 
 
 def find_lib_path():
-    """Find the path to xgboost dynamic library files.
+    """Find the path to boxhed_kernel dynamic library files.
 
     Returns
     -------
     lib_path: list(string)
-       List of all found library path to xgboost
+       List of all found library path to boxhed_kernel
     """
     curr_path = os.path.dirname(os.path.abspath(os.path.expanduser(__file__)))
     dll_path = [
         # normal, after installation `lib` is copied into Python package tree.
         os.path.join(curr_path, 'lib'),
         # editable installation, no copying is performed.
         os.path.join(curr_path, os.path.pardir, os.path.pardir, 'lib'),
-        # use libxgboost from a system prefix, if available.  This should be the last
+        # use libboxhed_kernel from a system prefix, if available.  This should be the last
         # option.
         os.path.join(sys.prefix, 'lib'),
     ]
 
     if sys.platform == 'win32':
         if platform.architecture()[0] == '64bit':
             dll_path.append(
@@ -37,28 +37,28 @@
             # directory here
             dll_path.append(os.path.join(curr_path, './windows/x64/Release/'))
         else:
             dll_path.append(os.path.join(curr_path, '../../windows/Release/'))
             # hack for pip installation when copy all parent source
             # directory here
             dll_path.append(os.path.join(curr_path, './windows/Release/'))
-        dll_path = [os.path.join(p, 'xgboost.dll') for p in dll_path]
+        dll_path = [os.path.join(p, 'boxhed_kernel.dll') for p in dll_path]
     elif sys.platform.startswith('linux') or sys.platform.startswith(
             'freebsd'):
-        dll_path = [os.path.join(p, 'libxgboost.so') for p in dll_path]
+        dll_path = [os.path.join(p, 'libboxhed_kernel.so') for p in dll_path]
     elif sys.platform == 'darwin':
-        dll_path = [os.path.join(p, 'libxgboost.dylib') for p in dll_path]
+        dll_path = [os.path.join(p, 'libboxhed_kernel.dylib') for p in dll_path]
     elif sys.platform == 'cygwin':
-        dll_path = [os.path.join(p, 'cygxgboost.dll') for p in dll_path]
+        dll_path = [os.path.join(p, 'cygboxhed_kernel.dll') for p in dll_path]
 
     lib_path = [p for p in dll_path if os.path.exists(p) and os.path.isfile(p)]
 
     # XGBOOST_BUILD_DOC is defined by sphinx conf.
     if not lib_path and not os.environ.get('XGBOOST_BUILD_DOC', False):
-        link = 'https://xgboost.readthedocs.io/en/latest/build.html'
+        link = 'https://boxhed_kernel.readthedocs.io/en/latest/build.html'
         msg = 'Cannot find XGBoost Library in the candidate path.  ' + \
             'List of candidates:\n- ' + ('\n- '.join(dll_path)) + \
             '\nXGBoost Python package path: ' + curr_path + \
             '\nsys.prefix: ' + sys.prefix + \
             '\nSee: ' + link + ' for installing XGBoost.'
         raise XGBoostLibraryNotFound(msg)
     return lib_path
```

### Comparing `boxhed_kernel-2.0.1/xgboost/plotting.py` & `boxhed_kernel-2.0.2/boxhed_kernel/plotting.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/xgboost/rabit.py` & `boxhed_kernel-2.0.2/boxhed_kernel/rabit.py`

 * *Files identical despite different names*

### Comparing `boxhed_kernel-2.0.1/xgboost/sklearn.py` & `boxhed_kernel-2.0.2/boxhed_kernel/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,30 @@
                      XGBClassifierBase, XGBRegressorBase, XGBoostLabelEncoder)
 
 
 def _objective_decorator(func):
     """Decorate an objective function
 
     Converts an objective function using the typical sklearn metrics
-    signature so that it is usable with ``xgboost.training.train``
+    signature so that it is usable with ``boxhed_kernel.training.train``
 
     Parameters
     ----------
     func: callable
         Expects a callable with signature ``func(y_true, y_pred)``:
 
         y_true: array_like of shape [n_samples]
             The target values
         y_pred: array_like of shape [n_samples]
             The predicted values
 
     Returns
     -------
     new_func: callable
-        The new objective function as expected by ``xgboost.training.train``.
+        The new objective function as expected by ``boxhed_kernel.training.train``.
         The signature is ``new_func(preds, dmatrix)``:
 
         preds: array_like, shape [n_samples]
             The predicted values
         dmatrix: ``DMatrix``
             The training set from which the labels will be extracted using
             ``dmatrix.get_label()``
@@ -70,15 +70,15 @@
         Specify which booster to use: gbtree, gblinear or dart.
     tree_method: string
         Specify which tree method to use.  Default to auto.  If this parameter
         is set to default, XGBoost will choose the most conservative option
         available.  It's recommended to study this option from parameters
         document.
     n_jobs : int
-        Number of parallel threads used to run xgboost.  When used with other Scikit-Learn
+        Number of parallel threads used to run boxhed_kernel.  When used with other Scikit-Learn
         algorithms like grid search, you may choose which algorithm to parallelize and
         balance the threads.  Creating thread contention will significantly slow dowm both
         algorithms.
     gamma : float
         Minimum loss reduction required to make a further partition on a leaf
         node of the tree.
     min_child_weight : float
@@ -125,15 +125,15 @@
     importance_type: string, default "gain"
         The feature importance type for the feature_importances\\_ property:
         either "gain", "weight", "cover", "total_gain" or "total_cover".
 
     \\*\\*kwargs : dict, optional
         Keyword arguments for XGBoost Booster object.  Full documentation of
         parameters can be found here:
-        https://github.com/dmlc/xgboost/blob/master/doc/parameter.rst.
+        https://github.com/dmlc/boxhed_kernel/blob/master/doc/parameter.rst.
         Attempting to set a parameter via the constructor args and \\*\\*kwargs
         dict simultaneously will result in a TypeError.
 
         .. note:: \\*\\*kwargs unsupported by scikit-learn
 
             \\*\\*kwargs is unsupported by scikit-learn.  We do not guarantee
             that parameters passed via this argument will interact properly
@@ -155,15 +155,15 @@
             grad: array_like of shape [n_samples]
                 The value of the gradient for each sample point.
             hess: array_like of shape [n_samples]
                 The value of the second derivative for each sample point
 '''
 
 
-def xgboost_model_doc(header, items, extra_parameters=None, end_note=None):
+def boxhed_kernel_model_doc(header, items, extra_parameters=None, end_note=None):
     '''Obtain documentation for Scikit-Learn wrappers
 
     Parameters
     ----------
     header: str
        An introducion to the class.
     items : list
@@ -196,15 +196,15 @@
         full_doc = [header + '\n\n']
         full_doc.extend(doc)
         cls.__doc__ = ''.join(full_doc)
         return cls
     return adddoc
 
 
-@xgboost_model_doc("""Implementation of the Scikit-Learn API for XGBoost.""",
+@boxhed_kernel_model_doc("""Implementation of the Scikit-Learn API for XGBoost.""",
                    ['estimators', 'model', 'objective'])
 class XGBModel(XGBModelBase):
     # pylint: disable=too-many-arguments, too-many-instance-attributes, missing-docstring
     def __init__(self, max_depth=None, learning_rate=None, n_estimators=100,
                  verbosity=None, objective=None, booster=None,
                  tree_method=None, n_jobs=None, gamma=None,
                  min_child_weight=None, max_delta_step=None, subsample=None,
@@ -294,30 +294,30 @@
         return train_dmatrix, evals
 
     def _more_tags(self):
         '''Tags used for scikit-learn data validation.'''
         return {'allow_nan': True, 'no_validation': True}
 
     def get_booster(self):
-        """Get the underlying xgboost Booster of this model.
+        """Get the underlying boxhed_kernel Booster of this model.
 
         This will raise an exception when fit was not called
 
         Returns
         -------
-        booster : a xgboost booster of underlying model
+        booster : a boxhed_kernel booster of underlying model
         """
         if not hasattr(self, '_Booster'):
             from sklearn.exceptions import NotFittedError
             raise NotFittedError('need to call fit or load_model beforehand')
         return self._Booster
 
     def set_params(self, **params):
         """Set the parameters of this estimator.  Modification of the sklearn method to
-        allow unknown kwargs. This allows using the full range of xgboost
+        allow unknown kwargs. This allows using the full range of boxhed_kernel
         parameters that are not defined as member variables in sklearn grid
         search.
 
         Returns
         -------
         self
 
@@ -383,41 +383,41 @@
                 if k in params.keys() and params[k] is None:
                     params[k] = parse_parameter(v)
         except ValueError:
             pass
         return params
 
     def get_xgb_params(self):
-        """Get xgboost specific parameters."""
+        """Get boxhed_kernel specific parameters."""
         params = self.get_params()
         # Parameters that should not go into native learner.
         wrapper_specific = {
             'importance_type', 'kwargs', 'missing', 'n_estimators', 'use_label_encoder'}
         filtered = dict()
         for k, v in params.items():
             if k not in wrapper_specific:
                 filtered[k] = v
         return filtered
 
     def get_num_boosting_rounds(self):
-        """Gets the number of xgboost boosting rounds."""
+        """Gets the number of boxhed_kernel boosting rounds."""
         return self.n_estimators
 
     def save_model(self, fname: str):
         """Save the model to a file.
 
         The model is saved in an XGBoost internal format which is universal
         among the various XGBoost interfaces. Auxiliary attributes of the
         Python Booster object (such as feature names) will not be saved.
 
           .. note::
 
             See:
 
-            https://xgboost.readthedocs.io/en/latest/tutorials/saving_model.html
+            https://boxhed_kernel.readthedocs.io/en/latest/tutorials/saving_model.html
 
         Parameters
         ----------
         fname : string
             Output file name
 
         """
@@ -794,15 +794,15 @@
             raise AttributeError(
                 'Intercept (bias) is not defined for Booster type {}'
                 .format(self.booster))
         b = self.get_booster()
         return np.array(json.loads(b.get_dump(dump_format='json')[0])['bias'])
 
 
-@xgboost_model_doc(
+@boxhed_kernel_model_doc(
     "Implementation of the scikit-learn API for XGBoost classification.",
     ['model', 'objective'], extra_parameters='''
     n_estimators : int
         Number of boosting rounds.
     use_label_encoder : bool
         (Deprecated) Use the label encoder from scikit-learn to encode the labels. For new code,
         we recommend that you set this parameter to False.
@@ -1066,15 +1066,15 @@
             evals_result = self.evals_result_
         else:
             raise XGBoostError('No results.')
 
         return evals_result
 
 
-@xgboost_model_doc(
+@boxhed_kernel_model_doc(
     "scikit-learn API for XGBoost random forest classification.",
     ['model', 'objective'],
     extra_parameters='''
     n_estimators : int
         Number of trees in random forest to fit.
     use_label_encoder : bool
         (Deprecated) Use the label encoder from scikit-learn to encode the labels. For new code,
@@ -1102,25 +1102,25 @@
         params['num_parallel_tree'] = self.n_estimators
         return params
 
     def get_num_boosting_rounds(self):
         return 1
 
 
-@xgboost_model_doc(
+@boxhed_kernel_model_doc(
     "Implementation of the scikit-learn API for XGBoost regression.",
     ['estimators', 'model', 'objective'])
 class XGBRegressor(XGBModel, XGBRegressorBase):
     # pylint: disable=missing-docstring
     @_deprecate_positional_args
     def __init__(self, *, objective="reg:squarederror", **kwargs):
         super().__init__(objective=objective, **kwargs)
 
 
-@xgboost_model_doc(
+@boxhed_kernel_model_doc(
     "scikit-learn API for XGBoost random forest regression.",
     ['model', 'objective'], extra_parameters='''
     n_estimators : int
         Number of trees in random forest to fit.
 ''')
 class XGBRFRegressor(XGBRegressor):
     # pylint: disable=missing-docstring
@@ -1136,15 +1136,15 @@
         params['num_parallel_tree'] = self.n_estimators
         return params
 
     def get_num_boosting_rounds(self):
         return 1
 
 
-@xgboost_model_doc(
+@boxhed_kernel_model_doc(
     'Implementation of the Scikit-Learn API for XGBoost Ranking.',
     ['estimators', 'model'],
     end_note='''
         Note
         ----
         A custom objective function is currently not supported by XGBRanker.
         Likewise, a custom metric function is not supported either.
```

### Comparing `boxhed_kernel-2.0.1/xgboost/tracker.py` & `boxhed_kernel-2.0.2/boxhed_kernel/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 This script is a variant of dmlc-core/dmlc_tracker/tracker.py,
-which is a specialized version for xgboost tasks.
+which is a specialized version for boxhed_kernel tasks.
 """
 
 # pylint: disable=invalid-name, missing-docstring, too-many-arguments, too-many-locals
 # pylint: disable=too-many-branches, too-many-statements, too-many-instance-attributes
 import socket
 import struct
 import time
```

### Comparing `boxhed_kernel-2.0.1/xgboost/training.py` & `boxhed_kernel-2.0.2/boxhed_kernel/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from . import rabit
 from . import callback
 
 
 def _configure_deprecated_callbacks(
         verbose_eval, early_stopping_rounds, maximize, start_iteration,
         num_boost_round, feval, evals_result, callbacks, show_stdv, cvfolds):
-    link = 'https://xgboost.readthedocs.io/en/latest/python/callbacks.html'
+    link = 'https://boxhed_kernel.readthedocs.io/en/latest/python/callbacks.html'
     warnings.warn(f'Old style callback is deprecated.  See: {link}', UserWarning)
     # Most of legacy advanced options becomes callbacks
     if early_stopping_rounds is not None:
         callbacks.append(callback.early_stop(early_stopping_rounds,
                                              maximize=maximize,
                                              verbose=bool(verbose_eval)))
     if isinstance(verbose_eval, bool) and verbose_eval:
```

