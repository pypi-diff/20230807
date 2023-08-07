# Comparing `tmp/xfem-2.1.2303.post6.dev0.tar.gz` & `tmp/xfem-2.1.2303.post8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfem-2.1.2303.post6.dev0.tar", last modified: Sun Jul  9 01:43:29 2023, max compression
+gzip compressed data, was "xfem-2.1.2303.post8.dev0.tar", last modified: Sun Jul  9 06:12:59 2023, max compression
```

## Comparing `xfem-2.1.2303.post6.dev0.tar` & `xfem-2.1.2303.post8.dev0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.920511 xfem-2.1.2303.post6.dev0/
--rw-r--r--   0 root         (0) root         (0)     7455 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7650 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-09 01:43:29.920511 xfem-2.1.2303.post6.dev0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8526 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-310/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.892511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/
--rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 01:36:55.000000 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-311/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.892511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/CompilerIdCXX/
--rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 01:40:24.000000 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-38/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.892511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/CompilerIdCXX/
--rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 01:33:25.000000 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-39/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.888511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.892511 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/CompilerIdCXX/
--rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 01:29:55.000000 xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.896511 xfem-2.1.2303.post6.dev0/cmake_modules/
--rw-r--r--   0 root         (0) root         (0)     1035 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cmake_modules/cmake_uninstall.cmake.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.900511 xfem-2.1.2303.post6.dev0/cutint/
--rw-r--r--   0 root         (0) root         (0)      214 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7745 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/cutintegral.cpp
--rw-r--r--   0 root         (0) root         (0)     4544 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/cutintegral.hpp
--rw-r--r--   0 root         (0) root         (0)     4241 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/fieldeval.cpp
--rw-r--r--   0 root         (0) root         (0)     4187 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/fieldeval.hpp
--rw-r--r--   0 root         (0) root         (0)    12108 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/lsetintdomain.cpp
--rw-r--r--   0 root         (0) root         (0)     6001 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/lsetintdomain.hpp
--rw-r--r--   0 root         (0) root         (0)     8068 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/mlsetintegration.cpp
--rw-r--r--   0 root         (0) root         (0)     1250 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/mlsetintegration.hpp
--rw-r--r--   0 root         (0) root         (0)    16622 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/python_cutint.cpp
--rw-r--r--   0 root         (0) root         (0)    18133 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/spacetimecutrule.cpp
--rw-r--r--   0 root         (0) root         (0)     1516 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/spacetimecutrule.hpp
--rw-r--r--   0 root         (0) root         (0)    39707 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/straightcutrule.cpp
--rw-r--r--   0 root         (0) root         (0)     7898 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/straightcutrule.hpp
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/xdecompose.cpp
--rw-r--r--   0 root         (0) root         (0)     3460 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/xdecompose.hpp
--rw-r--r--   0 root         (0) root         (0)    62867 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/xintegration.cpp
--rw-r--r--   0 root         (0) root         (0)    30845 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/cutint/xintegration.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.900511 xfem-2.1.2303.post6.dev0/demos/
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/demos/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.904511 xfem-2.1.2303.post6.dev0/lsetcurving/
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6959 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/calcpointshift.cpp
--rw-r--r--   0 root         (0) root         (0)     1911 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/calcpointshift.hpp
--rw-r--r--   0 root         (0) root         (0)     1391 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/lsetrefine.cpp
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/lsetrefine.hpp
--rw-r--r--   0 root         (0) root         (0)     7410 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/projshift.cpp
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/projshift.hpp
--rw-r--r--   0 root         (0) root         (0)     6600 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/python_lsetcurving.cpp
--rw-r--r--   0 root         (0) root         (0)     9915 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/shiftedevaluate.cpp
--rw-r--r--   0 root         (0) root         (0)     2204 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/shiftedevaluate.hpp
--rw-r--r--   0 root         (0) root         (0)     4351 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/shiftintegrators.cpp
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/lsetcurving/shiftintegrators.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.920511 xfem-2.1.2303.post6.dev0/python/
--rw-r--r--   0 root         (0) root         (0)     2673 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/python/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    39498 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15725 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/python/cutmg.py
--rw-r--r--   0 root         (0) root         (0)    19045 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/python/lset_spacetime.py
--rw-r--r--   0 root         (0) root         (0)    12837 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/python/lsetcurv.py
--rw-r--r--   0 root         (0) root         (0)    18823 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/python/mlset.py
--rw-r--r--   0 root         (0) root         (0)     1224 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/python/ngs_check.py
--rw-r--r--   0 root         (0) root         (0)     1413 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/python/python_ngsxfem.cpp
--rw-r--r--   0 root         (0) root         (0)     1517 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/python/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 01:43:29.920511 xfem-2.1.2303.post6.dev0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     5366 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.908511 xfem-2.1.2303.post6.dev0/spacetime/
--rw-r--r--   0 root         (0) root         (0)      152 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    12850 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/SpaceTimeFE.cpp
--rw-r--r--   0 root         (0) root         (0)     4721 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/SpaceTimeFE.hpp
--rw-r--r--   0 root         (0) root         (0)     9545 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/SpaceTimeFESpace.cpp
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/SpaceTimeFESpace.hpp
--rw-r--r--   0 root         (0) root         (0)     4530 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/diffopDt.cpp
--rw-r--r--   0 root         (0) root         (0)     4725 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/diffopDt.hpp
--rw-r--r--   0 root         (0) root         (0)    17384 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/python_spacetime.cpp
--rw-r--r--   0 root         (0) root         (0)    11113 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/spacetime_vtk.cpp
--rw-r--r--   0 root         (0) root         (0)     1763 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/spacetime_vtk.hpp
--rw-r--r--   0 root         (0) root         (0)     5304 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/timecf.cpp
--rw-r--r--   0 root         (0) root         (0)     2514 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/spacetime/timecf.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.908511 xfem-2.1.2303.post6.dev0/tests/
--rw-r--r--   0 root         (0) root         (0)     6002 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.912511 xfem-2.1.2303.post6.dev0/utils/
--rw-r--r--   0 root         (0) root         (0)      175 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1055 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/bitarraycf.cpp
--rw-r--r--   0 root         (0) root         (0)      622 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/bitarraycf.hpp
--rw-r--r--   0 root         (0) root         (0)     3248 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/ngsxstd.cpp
--rw-r--r--   0 root         (0) root         (0)     3563 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/ngsxstd.hpp
--rw-r--r--   0 root         (0) root         (0)     3960 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/p1interpol.cpp
--rw-r--r--   0 root         (0) root         (0)     1302 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/p1interpol.hpp
--rw-r--r--   0 root         (0) root         (0)    17275 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/python_utils.cpp
--rw-r--r--   0 root         (0) root         (0)     5777 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/restrictedblf.cpp
--rw-r--r--   0 root         (0) root         (0)     2073 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/restrictedblf.hpp
--rw-r--r--   0 root         (0) root         (0)     9284 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/restrictedfespace.cpp
--rw-r--r--   0 root         (0) root         (0)     6619 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/restrictedfespace.hpp
--rw-r--r--   0 root         (0) root         (0)    13017 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/xprolongation.cpp
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/utils/xprolongation.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.916511 xfem-2.1.2303.post6.dev0/xfem/
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    24796 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/aggregates.cpp
--rw-r--r--   0 root         (0) root         (0)     3377 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/aggregates.hpp
--rw-r--r--   0 root         (0) root         (0)    21010 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/cutinfo.cpp
--rw-r--r--   0 root         (0) root         (0)     6587 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/cutinfo.hpp
--rw-r--r--   0 root         (0) root         (0)    13722 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/ghostpenalty.cpp
--rw-r--r--   0 root         (0) root         (0)     3652 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/ghostpenalty.hpp
--rw-r--r--   0 root         (0) root         (0)    45185 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/python_xfem.cpp
--rw-r--r--   0 root         (0) root         (0)     4151 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/sFESpace.cpp
--rw-r--r--   0 root         (0) root         (0)     1612 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/sFESpace.hpp
--rw-r--r--   0 root         (0) root         (0)    76187 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/symboliccutbfi.cpp
--rw-r--r--   0 root         (0) root         (0)    19371 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/symboliccutbfi.hpp
--rw-r--r--   0 root         (0) root         (0)     4362 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/symboliccutlfi.cpp
--rw-r--r--   0 root         (0) root         (0)     1256 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/symboliccutlfi.hpp
--rw-r--r--   0 root         (0) root         (0)    19223 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/xFESpace.cpp
--rw-r--r--   0 root         (0) root         (0)     5786 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/xFESpace.hpp
--rw-r--r--   0 root         (0) root         (0)     2926 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/xfemdiffops.cpp
--rw-r--r--   0 root         (0) root         (0)     2150 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/xfemdiffops.hpp
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/xfiniteelement.cpp
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-09 01:29:22.000000 xfem-2.1.2303.post6.dev0/xfem/xfiniteelement.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 01:43:29.920511 xfem-2.1.2303.post6.dev0/xfem.egg-info/
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-09 01:43:29.000000 xfem-2.1.2303.post6.dev0/xfem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2865 2023-07-09 01:43:29.000000 xfem-2.1.2303.post6.dev0/xfem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 01:43:29.000000 xfem-2.1.2303.post6.dev0/xfem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-09 01:43:29.000000 xfem-2.1.2303.post6.dev0/xfem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-09 01:43:29.000000 xfem-2.1.2303.post6.dev0/xfem.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.629639 xfem-2.1.2303.post8.dev0/
+-rw-r--r--   0 root         (0) root         (0)     7455 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     7650 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-09 06:12:59.629639 xfem-2.1.2303.post8.dev0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8526 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.593639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/
+-rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 06:04:20.000000 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.593639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/CompilerIdCXX/
+-rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 06:08:52.000000 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.593639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/CompilerIdCXX/
+-rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 05:59:46.000000 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.589639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.597639 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/CompilerIdCXX/
+-rw-r--r--   0 root         (0) root         (0)    26294 2023-07-09 05:55:12.000000 xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.597639 xfem-2.1.2303.post8.dev0/cmake_modules/
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cmake_modules/cmake_uninstall.cmake.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.605639 xfem-2.1.2303.post8.dev0/cutint/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     7745 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/cutintegral.cpp
+-rw-r--r--   0 root         (0) root         (0)     4544 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/cutintegral.hpp
+-rw-r--r--   0 root         (0) root         (0)     4241 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/fieldeval.cpp
+-rw-r--r--   0 root         (0) root         (0)     4187 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/fieldeval.hpp
+-rw-r--r--   0 root         (0) root         (0)    12108 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/lsetintdomain.cpp
+-rw-r--r--   0 root         (0) root         (0)     6001 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/lsetintdomain.hpp
+-rw-r--r--   0 root         (0) root         (0)     8068 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/mlsetintegration.cpp
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/mlsetintegration.hpp
+-rw-r--r--   0 root         (0) root         (0)    16622 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/python_cutint.cpp
+-rw-r--r--   0 root         (0) root         (0)    18133 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/spacetimecutrule.cpp
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/spacetimecutrule.hpp
+-rw-r--r--   0 root         (0) root         (0)    39707 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/straightcutrule.cpp
+-rw-r--r--   0 root         (0) root         (0)     7898 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/straightcutrule.hpp
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/xdecompose.cpp
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/xdecompose.hpp
+-rw-r--r--   0 root         (0) root         (0)    62867 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/xintegration.cpp
+-rw-r--r--   0 root         (0) root         (0)    30845 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/cutint/xintegration.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.605639 xfem-2.1.2303.post8.dev0/demos/
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/demos/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.609639 xfem-2.1.2303.post8.dev0/lsetcurving/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6959 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/calcpointshift.cpp
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/calcpointshift.hpp
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/lsetrefine.cpp
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/lsetrefine.hpp
+-rw-r--r--   0 root         (0) root         (0)     7410 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/projshift.cpp
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/projshift.hpp
+-rw-r--r--   0 root         (0) root         (0)     6600 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/python_lsetcurving.cpp
+-rw-r--r--   0 root         (0) root         (0)     9915 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/shiftedevaluate.cpp
+-rw-r--r--   0 root         (0) root         (0)     2204 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/shiftedevaluate.hpp
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/shiftintegrators.cpp
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/lsetcurving/shiftintegrators.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.625639 xfem-2.1.2303.post8.dev0/python/
+-rw-r--r--   0 root         (0) root         (0)     2673 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    39498 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15725 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/cutmg.py
+-rw-r--r--   0 root         (0) root         (0)    19045 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/lset_spacetime.py
+-rw-r--r--   0 root         (0) root         (0)    12837 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/lsetcurv.py
+-rw-r--r--   0 root         (0) root         (0)    18823 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/mlset.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/ngs_check.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/python_ngsxfem.cpp
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/python/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 06:12:59.629639 xfem-2.1.2303.post8.dev0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     5366 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.613639 xfem-2.1.2303.post8.dev0/spacetime/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12850 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFE.cpp
+-rw-r--r--   0 root         (0) root         (0)     4721 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFE.hpp
+-rw-r--r--   0 root         (0) root         (0)     9545 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFESpace.cpp
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFESpace.hpp
+-rw-r--r--   0 root         (0) root         (0)     4530 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/diffopDt.cpp
+-rw-r--r--   0 root         (0) root         (0)     4725 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/diffopDt.hpp
+-rw-r--r--   0 root         (0) root         (0)    17384 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/python_spacetime.cpp
+-rw-r--r--   0 root         (0) root         (0)    11113 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/spacetime_vtk.cpp
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/spacetime_vtk.hpp
+-rw-r--r--   0 root         (0) root         (0)     5304 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/timecf.cpp
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/spacetime/timecf.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.613639 xfem-2.1.2303.post8.dev0/tests/
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.617639 xfem-2.1.2303.post8.dev0/utils/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/bitarraycf.cpp
+-rw-r--r--   0 root         (0) root         (0)      622 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/bitarraycf.hpp
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/ngsxstd.cpp
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/ngsxstd.hpp
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/p1interpol.cpp
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/p1interpol.hpp
+-rw-r--r--   0 root         (0) root         (0)    17275 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/python_utils.cpp
+-rw-r--r--   0 root         (0) root         (0)     5777 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/restrictedblf.cpp
+-rw-r--r--   0 root         (0) root         (0)     2073 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/restrictedblf.hpp
+-rw-r--r--   0 root         (0) root         (0)     9284 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/restrictedfespace.cpp
+-rw-r--r--   0 root         (0) root         (0)     6619 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/restrictedfespace.hpp
+-rw-r--r--   0 root         (0) root         (0)    13017 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/xprolongation.cpp
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/utils/xprolongation.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.625639 xfem-2.1.2303.post8.dev0/xfem/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    24796 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/aggregates.cpp
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/aggregates.hpp
+-rw-r--r--   0 root         (0) root         (0)    21010 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/cutinfo.cpp
+-rw-r--r--   0 root         (0) root         (0)     6587 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/cutinfo.hpp
+-rw-r--r--   0 root         (0) root         (0)    13722 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/ghostpenalty.cpp
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/ghostpenalty.hpp
+-rw-r--r--   0 root         (0) root         (0)    45185 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/python_xfem.cpp
+-rw-r--r--   0 root         (0) root         (0)     4151 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/sFESpace.cpp
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/sFESpace.hpp
+-rw-r--r--   0 root         (0) root         (0)    76187 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/symboliccutbfi.cpp
+-rw-r--r--   0 root         (0) root         (0)    19371 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/symboliccutbfi.hpp
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/symboliccutlfi.cpp
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/symboliccutlfi.hpp
+-rw-r--r--   0 root         (0) root         (0)    19223 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xFESpace.cpp
+-rw-r--r--   0 root         (0) root         (0)     5786 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xFESpace.hpp
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xfemdiffops.cpp
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xfemdiffops.hpp
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xfiniteelement.cpp
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-09 05:54:24.000000 xfem-2.1.2303.post8.dev0/xfem/xfiniteelement.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 06:12:59.629639 xfem-2.1.2303.post8.dev0/xfem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-09 06:12:59.000000 xfem-2.1.2303.post8.dev0/xfem.egg-info/top_level.txt
```

### Comparing `xfem-2.1.2303.post6.dev0/CMakeLists.txt` & `xfem-2.1.2303.post8.dev0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/LICENSE` & `xfem-2.1.2303.post8.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/PKG-INFO` & `xfem-2.1.2303.post8.dev0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfem
-Version: 2.1.2303.post6.dev0
+Version: 2.1.2303.post8.dev0
 Summary: (ngs)xfem is an Add-on library to Netgen/NGSolve for unfitted/cut FEM.
 Home-page: https://github.com/ngsxfem/ngsxfem
 Author: Christoph Lehrenfeld
 Author-email: lehrenfeld@math.uni-goettingen.de
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `xfem-2.1.2303.post6.dev0/README.md` & `xfem-2.1.2303.post8.dev0/README.md`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-310/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-311/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-38/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `xfem-2.1.2303.post8.dev0/build/temp.linux-x86_64-cpython-39/CMakeFiles/3.25.0/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cmake_modules/cmake_uninstall.cmake.in` & `xfem-2.1.2303.post8.dev0/cmake_modules/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/cutintegral.cpp` & `xfem-2.1.2303.post8.dev0/cutint/cutintegral.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/cutintegral.hpp` & `xfem-2.1.2303.post8.dev0/cutint/cutintegral.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/fieldeval.cpp` & `xfem-2.1.2303.post8.dev0/cutint/fieldeval.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/fieldeval.hpp` & `xfem-2.1.2303.post8.dev0/cutint/fieldeval.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/lsetintdomain.cpp` & `xfem-2.1.2303.post8.dev0/cutint/lsetintdomain.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/lsetintdomain.hpp` & `xfem-2.1.2303.post8.dev0/cutint/lsetintdomain.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/mlsetintegration.cpp` & `xfem-2.1.2303.post8.dev0/cutint/mlsetintegration.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/mlsetintegration.hpp` & `xfem-2.1.2303.post8.dev0/cutint/mlsetintegration.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/python_cutint.cpp` & `xfem-2.1.2303.post8.dev0/cutint/python_cutint.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/spacetimecutrule.cpp` & `xfem-2.1.2303.post8.dev0/cutint/spacetimecutrule.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/spacetimecutrule.hpp` & `xfem-2.1.2303.post8.dev0/cutint/spacetimecutrule.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/straightcutrule.cpp` & `xfem-2.1.2303.post8.dev0/cutint/straightcutrule.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/straightcutrule.hpp` & `xfem-2.1.2303.post8.dev0/cutint/straightcutrule.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/xdecompose.cpp` & `xfem-2.1.2303.post8.dev0/cutint/xdecompose.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/xdecompose.hpp` & `xfem-2.1.2303.post8.dev0/cutint/xdecompose.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/xintegration.cpp` & `xfem-2.1.2303.post8.dev0/cutint/xintegration.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/cutint/xintegration.hpp` & `xfem-2.1.2303.post8.dev0/cutint/xintegration.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/calcpointshift.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/calcpointshift.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/calcpointshift.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/calcpointshift.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/lsetrefine.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/lsetrefine.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/lsetrefine.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/lsetrefine.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/projshift.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/projshift.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/projshift.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/projshift.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/python_lsetcurving.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/python_lsetcurving.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/shiftedevaluate.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/shiftedevaluate.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/shiftedevaluate.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/shiftedevaluate.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/shiftintegrators.cpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/shiftintegrators.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/lsetcurving/shiftintegrators.hpp` & `xfem-2.1.2303.post8.dev0/lsetcurving/shiftintegrators.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/python/CMakeLists.txt` & `xfem-2.1.2303.post8.dev0/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/python/__init__.py` & `xfem-2.1.2303.post8.dev0/python/__init__.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/python/cutmg.py` & `xfem-2.1.2303.post8.dev0/python/cutmg.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/python/lset_spacetime.py` & `xfem-2.1.2303.post8.dev0/python/lset_spacetime.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/python/lsetcurv.py` & `xfem-2.1.2303.post8.dev0/python/lsetcurv.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/python/mlset.py` & `xfem-2.1.2303.post8.dev0/python/mlset.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/python/ngs_check.py` & `xfem-2.1.2303.post8.dev0/python/ngs_check.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/python/python_ngsxfem.cpp` & `xfem-2.1.2303.post8.dev0/python/python_ngsxfem.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/python/utils.py` & `xfem-2.1.2303.post8.dev0/python/utils.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/setup.py` & `xfem-2.1.2303.post8.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/SpaceTimeFE.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFE.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/SpaceTimeFE.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFE.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/SpaceTimeFESpace.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFESpace.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/SpaceTimeFESpace.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/SpaceTimeFESpace.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/diffopDt.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/diffopDt.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/diffopDt.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/diffopDt.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/python_spacetime.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/python_spacetime.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/spacetime_vtk.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/spacetime_vtk.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/spacetime_vtk.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/spacetime_vtk.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/timecf.cpp` & `xfem-2.1.2303.post8.dev0/spacetime/timecf.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/spacetime/timecf.hpp` & `xfem-2.1.2303.post8.dev0/spacetime/timecf.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/tests/CMakeLists.txt` & `xfem-2.1.2303.post8.dev0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/bitarraycf.cpp` & `xfem-2.1.2303.post8.dev0/utils/bitarraycf.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/bitarraycf.hpp` & `xfem-2.1.2303.post8.dev0/utils/bitarraycf.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/ngsxstd.cpp` & `xfem-2.1.2303.post8.dev0/utils/ngsxstd.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/ngsxstd.hpp` & `xfem-2.1.2303.post8.dev0/utils/ngsxstd.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/p1interpol.cpp` & `xfem-2.1.2303.post8.dev0/utils/p1interpol.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/p1interpol.hpp` & `xfem-2.1.2303.post8.dev0/utils/p1interpol.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/python_utils.cpp` & `xfem-2.1.2303.post8.dev0/utils/python_utils.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/restrictedblf.cpp` & `xfem-2.1.2303.post8.dev0/utils/restrictedblf.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/restrictedblf.hpp` & `xfem-2.1.2303.post8.dev0/utils/restrictedblf.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/restrictedfespace.cpp` & `xfem-2.1.2303.post8.dev0/utils/restrictedfespace.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/restrictedfespace.hpp` & `xfem-2.1.2303.post8.dev0/utils/restrictedfespace.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/xprolongation.cpp` & `xfem-2.1.2303.post8.dev0/utils/xprolongation.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/utils/xprolongation.hpp` & `xfem-2.1.2303.post8.dev0/utils/xprolongation.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/aggregates.cpp` & `xfem-2.1.2303.post8.dev0/xfem/aggregates.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/aggregates.hpp` & `xfem-2.1.2303.post8.dev0/xfem/aggregates.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/cutinfo.cpp` & `xfem-2.1.2303.post8.dev0/xfem/cutinfo.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/cutinfo.hpp` & `xfem-2.1.2303.post8.dev0/xfem/cutinfo.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/ghostpenalty.cpp` & `xfem-2.1.2303.post8.dev0/xfem/ghostpenalty.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/ghostpenalty.hpp` & `xfem-2.1.2303.post8.dev0/xfem/ghostpenalty.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/python_xfem.cpp` & `xfem-2.1.2303.post8.dev0/xfem/python_xfem.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/sFESpace.cpp` & `xfem-2.1.2303.post8.dev0/xfem/sFESpace.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/sFESpace.hpp` & `xfem-2.1.2303.post8.dev0/xfem/sFESpace.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/symboliccutbfi.cpp` & `xfem-2.1.2303.post8.dev0/xfem/symboliccutbfi.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/symboliccutbfi.hpp` & `xfem-2.1.2303.post8.dev0/xfem/symboliccutbfi.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/symboliccutlfi.cpp` & `xfem-2.1.2303.post8.dev0/xfem/symboliccutlfi.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/symboliccutlfi.hpp` & `xfem-2.1.2303.post8.dev0/xfem/symboliccutlfi.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/xFESpace.cpp` & `xfem-2.1.2303.post8.dev0/xfem/xFESpace.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/xFESpace.hpp` & `xfem-2.1.2303.post8.dev0/xfem/xFESpace.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/xfemdiffops.cpp` & `xfem-2.1.2303.post8.dev0/xfem/xfemdiffops.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/xfemdiffops.hpp` & `xfem-2.1.2303.post8.dev0/xfem/xfemdiffops.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/xfiniteelement.cpp` & `xfem-2.1.2303.post8.dev0/xfem/xfiniteelement.cpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem/xfiniteelement.hpp` & `xfem-2.1.2303.post8.dev0/xfem/xfiniteelement.hpp`

 * *Files identical despite different names*

### Comparing `xfem-2.1.2303.post6.dev0/xfem.egg-info/PKG-INFO` & `xfem-2.1.2303.post8.dev0/xfem.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfem
-Version: 2.1.2303.post6.dev0
+Version: 2.1.2303.post8.dev0
 Summary: (ngs)xfem is an Add-on library to Netgen/NGSolve for unfitted/cut FEM.
 Home-page: https://github.com/ngsxfem/ngsxfem
 Author: Christoph Lehrenfeld
 Author-email: lehrenfeld@math.uni-goettingen.de
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `xfem-2.1.2303.post6.dev0/xfem.egg-info/SOURCES.txt` & `xfem-2.1.2303.post8.dev0/xfem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

