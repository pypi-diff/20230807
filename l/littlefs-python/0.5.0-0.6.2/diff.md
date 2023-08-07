# Comparing `tmp/littlefs-python-0.5.0.tar.gz` & `tmp/littlefs-python-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littlefs-python-0.5.0.tar", last modified: Fri May 26 23:21:06 2023, max compression
+gzip compressed data, was "littlefs-python-0.6.2.tar", last modified: Mon Aug  7 14:31:51 2023, max compression
```

## Comparing `littlefs-python-0.5.0.tar` & `littlefs-python-0.6.2.tar`

### file list

```diff
@@ -1,139 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/ci/
--rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/ci/build-wheels.sh
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/ci/download_release_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/doc8.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/examples/mkfsimg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/examples/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.git
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/littlefs/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.github/workflows/post-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.github/workflows/status.yml
--rw-r--r--   0 runner    (1001) docker     (123)    26975 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    96233 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/DESIGN.md
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    33650 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/SPEC.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/bd/
--rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_emubd.c
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_emubd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_filebd.c
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_filebd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_rambd.c
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/bd/lfs_rambd.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/benches/bench_dir.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/benches/bench_file.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/benches/bench_superblock.toml
--rw-r--r--   0 runner    (1001) docker     (123)   184603 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/lfs.c
--rw-r--r--   0 runner    (1001) docker     (123)    23801 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/lfs.h
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/lfs_util.c
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/lfs_util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.314197 littlefs-python-0.5.0/littlefs/runners/
--rw-r--r--   0 runner    (1001) docker     (123)    67872 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/runners/bench_runner.c
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/runners/bench_runner.h
--rw-r--r--   0 runner    (1001) docker     (123)    91607 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/runners/test_runner.c
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/runners/test_runner.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.318197 littlefs-python-0.5.0/littlefs/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    52054 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/bench.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5401 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/changeprefix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23095 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/code.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27397 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/cov.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22943 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45193 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/perf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44308 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/perfbd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54030 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    41869 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/plotmpl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15011 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/prettyasserts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/readblock.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12631 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/readmdir.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6357 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/readtree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24367 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/stack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21064 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/structs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25393 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/summary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5275 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/tailpipe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1993 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/teepipe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54598 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31069 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/tracebd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8135 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/scripts/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.318197 littlefs-python-0.5.0/littlefs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_alloc.toml
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_attrs.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_badblocks.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_bd.toml
--rw-r--r--   0 runner    (1001) docker     (123)    41114 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_compat.toml
--rw-r--r--   0 runner    (1001) docker     (123)    32864 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_dirs.toml
--rw-r--r--   0 runner    (1001) docker     (123)    22546 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_entries.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_evil.toml
--rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_exhaustion.toml
--rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_files.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_interspersed.toml
--rw-r--r--   0 runner    (1001) docker     (123)    70817 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_move.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_orphans.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_paths.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_powerloss.toml
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_relocations.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_seek.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_superblocks.toml
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-05-26 23:21:01.000000 littlefs-python-0.5.0/littlefs/tests/test_truncate.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.310197 littlefs-python-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/src/littlefs/
--rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   667029 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs/lfs.c
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/lfs.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/lfs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/lfs.pyx
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/src/littlefs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/src/littlefs_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 23:21:06.000000 littlefs-python-0.5.0/src/littlefs_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 23:21:06.322197 littlefs-python-0.5.0/test/lfs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/lfs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/lfs/test_dir_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/lfs/test_file_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/lfs/test_fs_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_remove_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-26 23:21:00.000000 littlefs-python-0.5.0/test/test_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.852599 littlefs-python-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-08-07 14:31:51.852599 littlefs-python-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/ci/build-wheels.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/ci/download_release_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/docs/doc8.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/examples/mkfsimg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/examples/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/littlefs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/.git
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/littlefs/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.844600 littlefs-python-0.6.2/littlefs/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/.github/workflows/post-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/.github/workflows/status.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    28922 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    96233 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/DESIGN.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33650 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/SPEC.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.844600 littlefs-python-0.6.2/littlefs/bd/
+-rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/bd/lfs_emubd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/bd/lfs_emubd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/bd/lfs_filebd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/bd/lfs_filebd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/bd/lfs_rambd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/bd/lfs_rambd.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.844600 littlefs-python-0.6.2/littlefs/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/benches/bench_dir.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/benches/bench_file.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/benches/bench_superblock.toml
+-rw-r--r--   0 runner    (1001) docker     (123)   187983 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/lfs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/lfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/lfs_util.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/lfs_util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.844600 littlefs-python-0.6.2/littlefs/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)    67872 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/runners/bench_runner.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/runners/bench_runner.h
+-rw-r--r--   0 runner    (1001) docker     (123)    92022 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/runners/test_runner.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/runners/test_runner.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.844600 littlefs-python-0.6.2/littlefs/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52054 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/bench.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5401 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/changeprefix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23095 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/code.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27397 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/cov.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22943 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45193 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/perf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44308 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/perfbd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54030 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41869 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/plotmpl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15011 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/prettyasserts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/readblock.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12631 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/readmdir.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6357 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/readtree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24367 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/stack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21064 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/structs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25393 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5275 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/tailpipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1993 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/teepipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54598 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31069 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/tracebd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8135 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/scripts/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.848600 littlefs-python-0.6.2/littlefs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_alloc.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_attrs.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_badblocks.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_bd.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    42929 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_compat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    32864 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_dirs.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    22546 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_entries.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_evil.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_exhaustion.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_files.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_interspersed.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    70817 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_move.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_orphans.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_paths.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_powerloss.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_relocations.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_seek.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_superblocks.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-08-07 14:31:45.000000 littlefs-python-0.6.2/littlefs/tests/test_truncate.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:31:51.852599 littlefs-python-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.840600 littlefs-python-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.848600 littlefs-python-0.6.2/src/littlefs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/src/littlefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/src/littlefs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/src/littlefs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1606761 2023-08-07 14:31:51.000000 littlefs-python-0.6.2/src/littlefs/lfs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/src/littlefs/lfs.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/src/littlefs/lfs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/src/littlefs/lfs.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/src/littlefs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.848600 littlefs-python-0.6.2/src/littlefs_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-08-07 14:31:51.000000 littlefs-python-0.6.2/src/littlefs_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-08-07 14:31:51.000000 littlefs-python-0.6.2/src/littlefs_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:31:51.000000 littlefs-python-0.6.2/src/littlefs_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:31:51.000000 littlefs-python-0.6.2/src/littlefs_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 14:31:51.000000 littlefs-python-0.6.2/src/littlefs_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.852599 littlefs-python-0.6.2/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:51.852599 littlefs-python-0.6.2/test/lfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/lfs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/lfs/test_dir_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/lfs/test_file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/lfs/test_fs_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/test_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/test_multiversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/test_remove_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-07 14:31:44.000000 littlefs-python-0.6.2/test/test_walk.py
```

### Comparing `littlefs-python-0.5.0/.github/workflows/run-tests.yml` & `littlefs-python-0.6.2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/LICENSE` & `littlefs-python-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/PKG-INFO` & `littlefs-python-0.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: littlefs-python
-Version: 0.5.0
+Version: 0.6.2
 Summary: A python wrapper for littlefs
 Home-page: https://github.com/jrast/littlefs-python
 Author: Jürg Rast
 Author-email: juergr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -86,28 +91,32 @@
     As littlefs_ is bundled with the package you will need to install the correct version of
     this package in successfully read or create images for your embedded system. If you start
     from scratch the latest version is recommeded.
 
     .. csv-table::
         :header: "Package Version", "LittleFS Version", "LittleFS File System Version"
 
-        0.6.0, 2.6.1, 2.1
-        0.5.0, 2.4.1, 2.0
+        0.6.0, 2.7.0, 2.0 / 2.1 [#f1]_
+        0.5.0, 2.6.1, 2.1
         0.4.0, 2.2.1, 2.0
+        0.3.0, 2.2.1, 2.0
+
+    .. [#f1] See ``test/test_multiversion.py`` for examples.
 
 
 This is as simple as it can be::
 
     pip install littlefs-python
 
 At the moment wheels (which require no build) are provided for the following platforms,
 on other platforms the source package is used and a compiler is required:
 
- - Linux: Python 3.6 - 3.10 / 32- & 64-bit
- - Windows: Python 3.6 - 3.10 / 32- & 64-bit
+ - Linux: Python 3.6 - 3.11 / x86_64, arm64
+ - MacOS: Python 3.6 - 3.11 / x86_64, arm64
+ - Windows: Python 3.6 - 3.11 / 32- & 64-bit
 
 
 Development Setup
 =================
 
 Start by checking out the source repository of littlefs-python::
```

### Comparing `littlefs-python-0.5.0/README.rst` & `littlefs-python-0.6.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -67,28 +67,32 @@
     As littlefs_ is bundled with the package you will need to install the correct version of
     this package in successfully read or create images for your embedded system. If you start
     from scratch the latest version is recommeded.
 
     .. csv-table::
         :header: "Package Version", "LittleFS Version", "LittleFS File System Version"
 
-        0.6.0, 2.6.1, 2.1
-        0.5.0, 2.4.1, 2.0
+        0.6.0, 2.7.0, 2.0 / 2.1 [#f1]_
+        0.5.0, 2.6.1, 2.1
         0.4.0, 2.2.1, 2.0
+        0.3.0, 2.2.1, 2.0
+
+    .. [#f1] See ``test/test_multiversion.py`` for examples.
 
 
 This is as simple as it can be::
 
     pip install littlefs-python
 
 At the moment wheels (which require no build) are provided for the following platforms,
 on other platforms the source package is used and a compiler is required:
 
- - Linux: Python 3.6 - 3.10 / 32- & 64-bit
- - Windows: Python 3.6 - 3.10 / 32- & 64-bit
+ - Linux: Python 3.6 - 3.11 / x86_64, arm64
+ - MacOS: Python 3.6 - 3.11 / x86_64, arm64
+ - Windows: Python 3.6 - 3.11 / 32- & 64-bit
 
 
 Development Setup
 =================
 
 Start by checking out the source repository of littlefs-python::
```

### Comparing `littlefs-python-0.5.0/ci/build-wheels.sh` & `littlefs-python-0.6.2/ci/build-wheels.sh`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/ci/download_release_files.py` & `littlefs-python-0.6.2/ci/download_release_files.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/docs/Makefile` & `littlefs-python-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/docs/conf.py` & `littlefs-python-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/docs/examples/index.rst` & `littlefs-python-0.6.2/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/docs/make.bat` & `littlefs-python-0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/docs/usage.rst` & `littlefs-python-0.6.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/examples/mkfsimg.py` & `littlefs-python-0.6.2/examples/mkfsimg.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/examples/walk.py` & `littlefs-python-0.6.2/examples/walk.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/.github/workflows/post-release.yml` & `littlefs-python-0.6.2/littlefs/.github/workflows/post-release.yml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/.github/workflows/release.yml` & `littlefs-python-0.6.2/littlefs/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
           # build table for GitHub
           declare -A table
 
           # sizes table
           i=0
           j=0
-          for c in "" readonly threadsafe migrate error-asserts
+          for c in "" readonly threadsafe multiversion migrate error-asserts
           do
             # per-config results
             c_or_default=${c:-default}
             c_camel=${c_or_default^}
             table[$i,$j]=$c_camel
             ((j+=1))
```

### Comparing `littlefs-python-0.5.0/littlefs/.github/workflows/status.yml` & `littlefs-python-0.6.2/littlefs/.github/workflows/status.yml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/.github/workflows/test.yml` & `littlefs-python-0.6.2/littlefs/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -166,14 +166,35 @@
             -fdata=data_size \
             -fstack=stack_limit --max=stack_limit
           mkdir -p sizes
           cp lfs.code.csv sizes/${{matrix.arch}}-threadsafe.code.csv
           cp lfs.data.csv sizes/${{matrix.arch}}-threadsafe.data.csv
           cp lfs.stack.csv sizes/${{matrix.arch}}-threadsafe.stack.csv
           cp lfs.structs.csv sizes/${{matrix.arch}}-threadsafe.structs.csv
+      - name: sizes-multiversion
+        run: |
+          make clean
+          CFLAGS="$CFLAGS \
+            -DLFS_NO_ASSERT \
+            -DLFS_NO_DEBUG \
+            -DLFS_NO_WARN \
+            -DLFS_NO_ERROR \
+            -DLFS_MULTIVERSION" \
+            make lfs.code.csv lfs.data.csv lfs.stack.csv lfs.structs.csv
+          ./scripts/structs.py -u lfs.structs.csv
+          ./scripts/summary.py lfs.code.csv lfs.data.csv lfs.stack.csv \
+            -bfunction \
+            -fcode=code_size \
+            -fdata=data_size \
+            -fstack=stack_limit --max=stack_limit
+          mkdir -p sizes
+          cp lfs.code.csv sizes/${{matrix.arch}}-multiversion.code.csv
+          cp lfs.data.csv sizes/${{matrix.arch}}-multiversion.data.csv
+          cp lfs.stack.csv sizes/${{matrix.arch}}-multiversion.stack.csv
+          cp lfs.structs.csv sizes/${{matrix.arch}}-multiversion.structs.csv
       - name: sizes-migrate
         run: |
           make clean
           CFLAGS="$CFLAGS \
             -DLFS_NO_ASSERT \
             -DLFS_NO_DEBUG \
             -DLFS_NO_WARN \
@@ -349,14 +370,50 @@
           pip3 install toml
           gcc --version
           python3 --version
       - name: test-no-intrinsics
         run: |
           CFLAGS="$CFLAGS -DLFS_NO_INTRINSICS" make test
 
+  # run LFS_MULTIVERSION tests
+  test-multiversion:
+    runs-on: ubuntu-22.04
+    steps:
+      - uses: actions/checkout@v2
+      - name: install
+        run: |
+          # need a few things
+          sudo apt-get update -qq
+          sudo apt-get install -qq gcc python3 python3-pip
+          pip3 install toml
+          gcc --version
+          python3 --version
+      - name: test-multiversion
+        run: |
+          CFLAGS="$CFLAGS -DLFS_MULTIVERSION" make test
+
+  # run tests on the older version lfs2.0
+  test-lfs2_0:
+    runs-on: ubuntu-22.04
+    steps:
+      - uses: actions/checkout@v2
+      - name: install
+        run: |
+          # need a few things
+          sudo apt-get update -qq
+          sudo apt-get install -qq gcc python3 python3-pip
+          pip3 install toml
+          gcc --version
+          python3 --version
+      - name: test-lfs2_0
+        run: |
+          CFLAGS="$CFLAGS -DLFS_MULTIVERSION" \
+          TESTFLAGS="$TESTFLAGS -DDISK_VERSION=0x00020000" \
+            make test
+
   # run under Valgrind to check for memory errors
   test-valgrind:
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v2
       - name: install
         run: |
@@ -367,15 +424,16 @@
           gcc --version
           python3 --version
           valgrind --version
       # Valgrind takes a while with diminishing value, so only test
       # on one geometry
       - name: test-valgrind
         run: |
-          TESTFLAGS="$TESTFLAGS --valgrind -Gdefault -Pnone" make test
+          TESTFLAGS="$TESTFLAGS --valgrind --context=1024 -Gdefault -Pnone" \
+            make test
 
   # test that compilation is warning free under clang
   # run with Clang, mostly to check for Clang-specific warnings
   test-clang:
     runs-on: ubuntu-22.04
     steps:
       - uses: actions/checkout@v2
@@ -680,15 +738,15 @@
 
           # build table for GitHub
           declare -A table
 
           # sizes table
           i=0
           j=0
-          for c in "" readonly threadsafe migrate error-asserts
+          for c in "" readonly threadsafe multiversion migrate error-asserts
           do
             # per-config results
             c_or_default=${c:-default}
             c_camel=${c_or_default^}
             table[$i,$j]=$c_camel
             ((j+=1))
```

### Comparing `littlefs-python-0.5.0/littlefs/DESIGN.md` & `littlefs-python-0.6.2/littlefs/DESIGN.md`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/LICENSE.md` & `littlefs-python-0.6.2/littlefs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/Makefile` & `littlefs-python-0.6.2/littlefs/Makefile`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/README.md` & `littlefs-python-0.6.2/littlefs/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -246,14 +246,18 @@
   likely outperform littlefs on small memories such as the internal flash on
   microcontrollers.
 
 - [Dhara] - An interesting NAND flash translation layer designed for small
   MCUs. It offers static wear-leveling and power-resilience with only a fixed
   _O(|address|)_ pointer structure stored on each block and in RAM.
 
+- [ChaN's FatFs] - A lightweight reimplementation of the infamous FAT filesystem
+  for microcontroller-scale devices. Due to limitations of FAT it can't provide
+  power-loss resilience, but it does allow easy interop with PCs.
+
 - [chamelon] - A pure-OCaml implementation of (most of) littlefs, designed for
   use with the MirageOS library operating system project. It is interoperable
   with the reference implementation, with some caveats.
 
 [BSD-3-Clause]: https://spdx.org/licenses/BSD-3-Clause.html
 [littlefs-disk-img-viewer]: https://github.com/tniessen/littlefs-disk-img-viewer
 [littlefs-fuse]: https://github.com/geky/littlefs-fuse
@@ -262,10 +266,11 @@
 [littlefs-js-demo]:http://littlefs.geky.net/demo.html
 [mklfs]: https://github.com/whitecatboard/Lua-RTOS-ESP32/tree/master/components/mklfs/src
 [Lua RTOS]: https://github.com/whitecatboard/Lua-RTOS-ESP32
 [Mbed OS]: https://github.com/armmbed/mbed-os
 [LittleFileSystem]: https://os.mbed.com/docs/mbed-os/latest/apis/littlefilesystem.html
 [SPIFFS]: https://github.com/pellepl/spiffs
 [Dhara]: https://github.com/dlbeer/dhara
+[ChaN's FatFs]: http://elm-chan.org/fsw/ff/00index_e.html
 [littlefs-python]: https://pypi.org/project/littlefs-python/
 [littlefs2-rust]: https://crates.io/crates/littlefs2
 [chamelon]: https://github.com/yomimono/chamelon
```

### Comparing `littlefs-python-0.5.0/littlefs/SPEC.md` & `littlefs-python-0.6.2/littlefs/SPEC.md`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/bd/lfs_emubd.c` & `littlefs-python-0.6.2/littlefs/bd/lfs_emubd.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/bd/lfs_emubd.h` & `littlefs-python-0.6.2/littlefs/bd/lfs_emubd.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/bd/lfs_filebd.c` & `littlefs-python-0.6.2/littlefs/bd/lfs_filebd.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/bd/lfs_filebd.h` & `littlefs-python-0.6.2/littlefs/bd/lfs_filebd.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/bd/lfs_rambd.c` & `littlefs-python-0.6.2/littlefs/bd/lfs_rambd.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/bd/lfs_rambd.h` & `littlefs-python-0.6.2/littlefs/bd/lfs_rambd.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/benches/bench_dir.toml` & `littlefs-python-0.6.2/littlefs/benches/bench_dir.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/benches/bench_file.toml` & `littlefs-python-0.6.2/littlefs/benches/bench_file.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/benches/bench_superblock.toml` & `littlefs-python-0.6.2/littlefs/benches/bench_superblock.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/lfs.c` & `littlefs-python-0.6.2/littlefs/lfs.c`

 * *Files 1% similar despite different names*

```diff
@@ -411,19 +411,19 @@
 static inline uint8_t lfs_gstate_getorphans(const lfs_gstate_t *a) {
     return lfs_tag_size(a->tag) & 0x1ff;
 }
 
 static inline bool lfs_gstate_hasmove(const lfs_gstate_t *a) {
     return lfs_tag_type1(a->tag);
 }
+#endif
 
 static inline bool lfs_gstate_needssuperblock(const lfs_gstate_t *a) {
     return lfs_tag_size(a->tag) >> 9;
 }
-#endif
 
 static inline bool lfs_gstate_hasmovehere(const lfs_gstate_t *a,
         const lfs_block_t *pair) {
     return lfs_tag_type1(a->tag) && lfs_pair_cmp(a->pair, pair) == 0;
 }
 
 static inline void lfs_gstate_fromle32(lfs_gstate_t *a) {
@@ -514,14 +514,36 @@
 }
 
 static void lfs_mlist_append(lfs_t *lfs, struct lfs_mlist *mlist) {
     mlist->next = lfs->mlist;
     lfs->mlist = mlist;
 }
 
+// some other filesystem operations
+static uint32_t lfs_fs_disk_version(lfs_t *lfs) {
+    (void)lfs;
+#ifdef LFS_MULTIVERSION
+    if (lfs->cfg->disk_version) {
+        return lfs->cfg->disk_version;
+    } else
+#endif
+    {
+        return LFS_DISK_VERSION;
+    }
+}
+
+static uint16_t lfs_fs_disk_version_major(lfs_t *lfs) {
+    return 0xffff & (lfs_fs_disk_version(lfs) >> 16);
+
+}
+
+static uint16_t lfs_fs_disk_version_minor(lfs_t *lfs) {
+    return 0xffff & (lfs_fs_disk_version(lfs) >> 0);
+}
+
 
 /// Internal operations predeclared here ///
 #ifndef LFS_READONLY
 static int lfs_dir_commit(lfs_t *lfs, lfs_mdir_t *dir,
         const struct lfs_mattr *attrs, int attrcount);
 static int lfs_dir_compact(lfs_t *lfs,
         lfs_mdir_t *dir, const struct lfs_mattr *attrs, int attrcount,
@@ -531,25 +553,26 @@
 static lfs_ssize_t lfs_file_rawwrite(lfs_t *lfs, lfs_file_t *file,
         const void *buffer, lfs_size_t size);
 static int lfs_file_rawsync(lfs_t *lfs, lfs_file_t *file);
 static int lfs_file_outline(lfs_t *lfs, lfs_file_t *file);
 static int lfs_file_flush(lfs_t *lfs, lfs_file_t *file);
 
 static int lfs_fs_deorphan(lfs_t *lfs, bool powerloss);
-static void lfs_fs_prepsuperblock(lfs_t *lfs, bool needssuperblock);
 static int lfs_fs_preporphans(lfs_t *lfs, int8_t orphans);
 static void lfs_fs_prepmove(lfs_t *lfs,
         uint16_t id, const lfs_block_t pair[2]);
 static int lfs_fs_pred(lfs_t *lfs, const lfs_block_t dir[2],
         lfs_mdir_t *pdir);
 static lfs_stag_t lfs_fs_parent(lfs_t *lfs, const lfs_block_t dir[2],
         lfs_mdir_t *parent);
 static int lfs_fs_forceconsistency(lfs_t *lfs);
 #endif
 
+static void lfs_fs_prepsuperblock(lfs_t *lfs, bool needssuperblock);
+
 #ifdef LFS_MIGRATE
 static int lfs1_traverse(lfs_t *lfs,
         int (*cb)(void*, lfs_block_t), void *data);
 #endif
 
 static int lfs_dir_rawrewind(lfs_t *lfs, lfs_dir_t *dir);
 
@@ -1106,15 +1129,16 @@
             }
 
             crc = lfs_crc(crc, &tag, sizeof(tag));
             tag = lfs_frombe32(tag) ^ ptag;
 
             // next commit not yet programmed?
             if (!lfs_tag_isvalid(tag)) {
-                maybeerased = true;
+                // we only might be erased if the last tag was a crc
+                maybeerased = (lfs_tag_type2(ptag) == LFS_TYPE_CCRC);
                 break;
             // out of range?
             } else if (off + lfs_tag_dsize(tag) > lfs->cfg->block_size) {
                 break;
             }
 
             ptag = tag;
@@ -1151,22 +1175,19 @@
                 dir->off = off + lfs_tag_dsize(tag);
                 dir->etag = ptag;
                 dir->count = tempcount;
                 dir->tail[0] = temptail[0];
                 dir->tail[1] = temptail[1];
                 dir->split = tempsplit;
 
-                // reset crc
+                // reset crc, hasfcrc
                 crc = 0xffffffff;
                 continue;
             }
 
-            // fcrc is only valid when last tag was a crc
-            hasfcrc = false;
-
             // crc the entry first, hopefully leaving it in the cache
             err = lfs_bd_crc(lfs,
                     NULL, &lfs->rcache, lfs->cfg->block_size,
                     dir->pair[0], off+sizeof(tag),
                     lfs_tag_dsize(tag)-sizeof(tag), &crc);
             if (err) {
                 if (err == LFS_ERR_CORRUPT) {
@@ -1252,28 +1273,41 @@
             lfs_pair_swap(dir->pair);
             dir->rev = revs[(r+1)%2];
             continue;
         }
 
         // did we end on a valid commit? we may have an erased block
         dir->erased = false;
-        if (maybeerased && hasfcrc && dir->off % lfs->cfg->prog_size == 0) {
-            // check for an fcrc matching the next prog's erased state, if
-            // this failed most likely a previous prog was interrupted, we
-            // need a new erase
-            uint32_t fcrc_ = 0xffffffff;
-            int err = lfs_bd_crc(lfs,
-                    NULL, &lfs->rcache, lfs->cfg->block_size,
-                    dir->pair[0], dir->off, fcrc.size, &fcrc_);
-            if (err && err != LFS_ERR_CORRUPT) {
-                return err;
-            }
+        if (maybeerased && dir->off % lfs->cfg->prog_size == 0) {
+        #ifdef LFS_MULTIVERSION
+            // note versions < lfs2.1 did not have fcrc tags, if
+            // we're < lfs2.1 treat missing fcrc as erased data
+            //
+            // we don't strictly need to do this, but otherwise writing
+            // to lfs2.0 disks becomes very inefficient
+            if (lfs_fs_disk_version(lfs) < 0x00020001) {
+                dir->erased = true;
+
+            } else
+        #endif
+            if (hasfcrc) {
+                // check for an fcrc matching the next prog's erased state, if
+                // this failed most likely a previous prog was interrupted, we
+                // need a new erase
+                uint32_t fcrc_ = 0xffffffff;
+                int err = lfs_bd_crc(lfs,
+                        NULL, &lfs->rcache, lfs->cfg->block_size,
+                        dir->pair[0], dir->off, fcrc.size, &fcrc_);
+                if (err && err != LFS_ERR_CORRUPT) {
+                    return err;
+                }
 
-            // found beginning of erased part?
-            dir->erased = (fcrc_ == fcrc.crc);
+                // found beginning of erased part?
+                dir->erased = (fcrc_ == fcrc.crc);
+            }
         }
 
         // synthetic move
         if (lfs_gstate_hasmovehere(&lfs->gdisk, dir->pair)) {
             if (lfs_tag_id(lfs->gdisk.tag) == lfs_tag_id(besttag)) {
                 besttag |= 0x80000000;
             } else if (besttag != -1 &&
@@ -1601,30 +1635,42 @@
             int err = lfs_bd_read(lfs,
                     NULL, &lfs->rcache, lfs->cfg->prog_size,
                     commit->block, noff, &eperturb, 1);
             if (err && err != LFS_ERR_CORRUPT) {
                 return err;
             }
 
-            // find the expected fcrc, don't bother avoiding a reread
-            // of the eperturb, it should still be in our cache
-            struct lfs_fcrc fcrc = {.size=lfs->cfg->prog_size, .crc=0xffffffff};
-            err = lfs_bd_crc(lfs,
-                    NULL, &lfs->rcache, lfs->cfg->prog_size,
-                    commit->block, noff, fcrc.size, &fcrc.crc);
-            if (err && err != LFS_ERR_CORRUPT) {
-                return err;
-            }
+        #ifdef LFS_MULTIVERSION
+            // unfortunately fcrcs break mdir fetching < lfs2.1, so only write
+            // these if we're a >= lfs2.1 filesystem
+            if (lfs_fs_disk_version(lfs) <= 0x00020000) {
+                // don't write fcrc
+            } else
+        #endif
+            {
+                // find the expected fcrc, don't bother avoiding a reread
+                // of the eperturb, it should still be in our cache
+                struct lfs_fcrc fcrc = {
+                    .size = lfs->cfg->prog_size,
+                    .crc = 0xffffffff
+                };
+                err = lfs_bd_crc(lfs,
+                        NULL, &lfs->rcache, lfs->cfg->prog_size,
+                        commit->block, noff, fcrc.size, &fcrc.crc);
+                if (err && err != LFS_ERR_CORRUPT) {
+                    return err;
+                }
 
-            lfs_fcrc_tole32(&fcrc);
-            err = lfs_dir_commitattr(lfs, commit,
-                    LFS_MKTAG(LFS_TYPE_FCRC, 0x3ff, sizeof(struct lfs_fcrc)),
-                    &fcrc);
-            if (err) {
-                return err;
+                lfs_fcrc_tole32(&fcrc);
+                err = lfs_dir_commitattr(lfs, commit,
+                        LFS_MKTAG(LFS_TYPE_FCRC, 0x3ff, sizeof(struct lfs_fcrc)),
+                        &fcrc);
+                if (err) {
+                    return err;
+                }
             }
         }
 
         // build commit crc
         struct {
             lfs_tag_t tag;
             uint32_t crc;
@@ -4047,14 +4093,23 @@
 
 
 /// Filesystem operations ///
 static int lfs_init(lfs_t *lfs, const struct lfs_config *cfg) {
     lfs->cfg = cfg;
     int err = 0;
 
+#ifdef LFS_MULTIVERSION
+    // this driver only supports minor version < current minor version
+    LFS_ASSERT(!lfs->cfg->disk_version || (
+            (0xffff & (lfs->cfg->disk_version >> 16))
+                    == LFS_DISK_VERSION_MAJOR
+                && (0xffff & (lfs->cfg->disk_version >> 0))
+                    <= LFS_DISK_VERSION_MINOR));
+#endif
+
     // check that bool is a truthy-preserving type
     //
     // note the most common reason for this failure is a before-c99 compiler,
     // which littlefs currently does not support
     LFS_ASSERT((bool)0x80000000);
 
     // validate that the lfs-cfg sizes were initiated properly before
@@ -4204,15 +4259,15 @@
         err = lfs_dir_alloc(lfs, &root);
         if (err) {
             goto cleanup;
         }
 
         // write one superblock
         lfs_superblock_t superblock = {
-            .version     = LFS_DISK_VERSION,
+            .version     = lfs_fs_disk_version(lfs),
             .block_size  = lfs->cfg->block_size,
             .block_count = lfs->cfg->block_count,
             .name_max    = lfs->name_max,
             .file_max    = lfs->file_max,
             .attr_max    = lfs->attr_max,
         };
 
@@ -4302,37 +4357,39 @@
                 goto cleanup;
             }
             lfs_superblock_fromle32(&superblock);
 
             // check version
             uint16_t major_version = (0xffff & (superblock.version >> 16));
             uint16_t minor_version = (0xffff & (superblock.version >>  0));
-            if ((major_version != LFS_DISK_VERSION_MAJOR ||
-                 minor_version > LFS_DISK_VERSION_MINOR)) {
+            if (major_version != lfs_fs_disk_version_major(lfs)
+                    || minor_version > lfs_fs_disk_version_minor(lfs)) {
                 LFS_ERROR("Invalid version "
                         "v%"PRIu16".%"PRIu16" != v%"PRIu16".%"PRIu16,
-                        major_version, minor_version,
-                        LFS_DISK_VERSION_MAJOR, LFS_DISK_VERSION_MINOR);
+                        major_version,
+                        minor_version,
+                        lfs_fs_disk_version_major(lfs),
+                        lfs_fs_disk_version_minor(lfs));
                 err = LFS_ERR_INVAL;
                 goto cleanup;
             }
 
             // found older minor version? set an in-device only bit in the
             // gstate so we know we need to rewrite the superblock before
             // the first write
-            if (minor_version < LFS_DISK_VERSION_MINOR) {
+            if (minor_version < lfs_fs_disk_version_minor(lfs)) {
                 LFS_DEBUG("Found older minor version "
                         "v%"PRIu16".%"PRIu16" < v%"PRIu16".%"PRIu16,
-                        major_version, minor_version,
-                        LFS_DISK_VERSION_MAJOR, LFS_DISK_VERSION_MINOR);
-            #ifndef LFS_READONLY
+                        major_version,
+                        minor_version,
+                        lfs_fs_disk_version_major(lfs),
+                        lfs_fs_disk_version_minor(lfs));
                 // note this bit is reserved on disk, so fetching more gstate
                 // will not interfere here
                 lfs_fs_prepsuperblock(lfs, true);
-            #endif
             }
 
             // check superblock configuration
             if (superblock.name_max) {
                 if (superblock.name_max > lfs->name_max) {
                     LFS_ERROR("Unsupported name_max (%"PRIu32" > %"PRIu32")",
                             superblock.name_max, lfs->name_max);
@@ -4417,14 +4474,50 @@
 
 static int lfs_rawunmount(lfs_t *lfs) {
     return lfs_deinit(lfs);
 }
 
 
 /// Filesystem filesystem operations ///
+static int lfs_fs_rawstat(lfs_t *lfs, struct lfs_fsinfo *fsinfo) {
+    // if the superblock is up-to-date, we must be on the most recent
+    // minor version of littlefs
+    if (!lfs_gstate_needssuperblock(&lfs->gstate)) {
+        fsinfo->disk_version = lfs_fs_disk_version(lfs);
+
+    // otherwise we need to read the minor version on disk
+    } else {
+        // fetch the superblock
+        lfs_mdir_t dir;
+        int err = lfs_dir_fetch(lfs, &dir, lfs->root);
+        if (err) {
+            return err;
+        }
+
+        lfs_superblock_t superblock;
+        lfs_stag_t tag = lfs_dir_get(lfs, &dir, LFS_MKTAG(0x7ff, 0x3ff, 0),
+                LFS_MKTAG(LFS_TYPE_INLINESTRUCT, 0, sizeof(superblock)),
+                &superblock);
+        if (tag < 0) {
+            return tag;
+        }
+        lfs_superblock_fromle32(&superblock);
+
+        // read the on-disk version
+        fsinfo->disk_version = superblock.version;
+    }
+
+    // other on-disk configuration, we cache all of these for internal use
+    fsinfo->name_max = lfs->name_max;
+    fsinfo->file_max = lfs->file_max;
+    fsinfo->attr_max = lfs->attr_max;
+
+    return 0;
+}
+
 int lfs_fs_rawtraverse(lfs_t *lfs,
         int (*cb)(void *data, lfs_block_t block), void *data,
         bool includeorphans) {
     // iterate over metadata pairs
     lfs_mdir_t dir = {.tail = {0, 1}};
 
 #ifdef LFS_MIGRATE
@@ -4627,20 +4720,18 @@
         }
     }
 
     return LFS_ERR_NOENT;
 }
 #endif
 
-#ifndef LFS_READONLY
 static void lfs_fs_prepsuperblock(lfs_t *lfs, bool needssuperblock) {
     lfs->gstate.tag = (lfs->gstate.tag & ~LFS_MKTAG(0, 0, 0x200))
             | (uint32_t)needssuperblock << 9;
 }
-#endif
 
 #ifndef LFS_READONLY
 static int lfs_fs_preporphans(lfs_t *lfs, int8_t orphans) {
     LFS_ASSERT(lfs_tag_size(lfs->gstate.tag) > 0x000 || orphans >= 0);
     LFS_ASSERT(lfs_tag_size(lfs->gstate.tag) < 0x1ff || orphans <= 0);
     lfs->gstate.tag += orphans;
     lfs->gstate.tag = ((lfs->gstate.tag & ~LFS_MKTAG(0x800, 0, 0)) |
@@ -4674,15 +4765,15 @@
     int err = lfs_dir_fetch(lfs, &root, lfs->root);
     if (err) {
         return err;
     }
 
     // write a new superblock
     lfs_superblock_t superblock = {
-        .version     = LFS_DISK_VERSION,
+        .version     = lfs_fs_disk_version(lfs),
         .block_size  = lfs->cfg->block_size,
         .block_count = lfs->cfg->block_count,
         .name_max    = lfs->name_max,
         .file_max    = lfs->file_max,
         .attr_max    = lfs->attr_max,
     };
 
@@ -4930,14 +5021,15 @@
     if (err) {
         return err;
     }
 
     return size;
 }
 
+
 #ifdef LFS_MIGRATE
 ////// Migration from littelfs v1 below this //////
 
 /// Version info ///
 
 // Software library version
 // Major (top-nibble), incremented on backwards incompatible changes
@@ -6049,14 +6141,28 @@
     err = lfs_dir_rawrewind(lfs, dir);
 
     LFS_TRACE("lfs_dir_rewind -> %d", err);
     LFS_UNLOCK(lfs->cfg);
     return err;
 }
 
+int lfs_fs_stat(lfs_t *lfs, struct lfs_fsinfo *fsinfo) {
+    int err = LFS_LOCK(lfs->cfg);
+    if (err) {
+        return err;
+    }
+    LFS_TRACE("lfs_fs_stat(%p, %p)", (void*)lfs, (void*)fsinfo);
+
+    err = lfs_fs_rawstat(lfs, fsinfo);
+
+    LFS_TRACE("lfs_fs_stat -> %d", err);
+    LFS_UNLOCK(lfs->cfg);
+    return err;
+}
+
 lfs_ssize_t lfs_fs_size(lfs_t *lfs) {
     int err = LFS_LOCK(lfs->cfg);
     if (err) {
         return err;
     }
     LFS_TRACE("lfs_fs_size(%p)", (void*)lfs);
```

### Comparing `littlefs-python-0.5.0/littlefs/lfs.h` & `littlefs-python-0.6.2/littlefs/lfs.h`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 /// Version info ///
 
 // Software library version
 // Major (top-nibble), incremented on backwards incompatible changes
 // Minor (bottom-nibble), incremented on feature additions
-#define LFS_VERSION 0x00020006
+#define LFS_VERSION 0x00020007
 #define LFS_VERSION_MAJOR (0xffff & (LFS_VERSION >> 16))
 #define LFS_VERSION_MINOR (0xffff & (LFS_VERSION >>  0))
 
 // Version of On-disk data structures
 // Major (top-nibble), incremented on backwards incompatible changes
 // Minor (bottom-nibble), incremented on feature additions
 #define LFS_DISK_VERSION 0x00020001
@@ -259,14 +259,22 @@
     lfs_size_t attr_max;
 
     // Optional upper limit on total space given to metadata pairs in bytes. On
     // devices with large blocks (e.g. 128kB) setting this to a low size (2-8kB)
     // can help bound the metadata compaction time. Must be <= block_size.
     // Defaults to block_size when zero.
     lfs_size_t metadata_max;
+
+#ifdef LFS_MULTIVERSION
+    // On-disk version to use when writing in the form of 16-bit major version
+    // + 16-bit minor version. This limiting metadata to what is supported by
+    // older minor versions. Note that some features will be lost. Defaults to 
+    // to the most recent minor version when zero.
+    uint32_t disk_version;
+#endif
 };
 
 // File info structure
 struct lfs_info {
     // Type of the file, either LFS_TYPE_REG or LFS_TYPE_DIR
     uint8_t type;
 
@@ -276,14 +284,29 @@
     // Name of the file stored as a null-terminated string. Limited to
     // LFS_NAME_MAX+1, which can be changed by redefining LFS_NAME_MAX to
     // reduce RAM. LFS_NAME_MAX is stored in superblock and must be
     // respected by other littlefs drivers.
     char name[LFS_NAME_MAX+1];
 };
 
+// Filesystem info structure
+struct lfs_fsinfo {
+    // On-disk version.
+    uint32_t disk_version;
+
+    // Upper limit on the length of file names in bytes.
+    lfs_size_t name_max;
+
+    // Upper limit on the size of files in bytes.
+    lfs_size_t file_max;
+
+    // Upper limit on the size of custom attributes in bytes.
+    lfs_size_t attr_max;
+};
+
 // Custom attribute structure, used to describe custom attributes
 // committed atomically during file writes.
 struct lfs_attr {
     // 8-bit type of attribute, provided by user and used to
     // identify the attribute
     uint8_t type;
 
@@ -655,14 +678,20 @@
 //
 // Returns a negative error code on failure.
 int lfs_dir_rewind(lfs_t *lfs, lfs_dir_t *dir);
 
 
 /// Filesystem-level filesystem operations
 
+// Find on-disk info about the filesystem
+//
+// Fills out the fsinfo structure based on the filesystem found on-disk.
+// Returns a negative error code on failure.
+int lfs_fs_stat(lfs_t *lfs, struct lfs_fsinfo *fsinfo);
+
 // Finds the current size of the filesystem
 //
 // Note: Result is best effort. If files share COW structures, the returned
 // size may be larger than the filesystem actually is.
 //
 // Returns the number of allocated blocks, or a negative error code on failure.
 lfs_ssize_t lfs_fs_size(lfs_t *lfs);
```

### Comparing `littlefs-python-0.5.0/littlefs/lfs_util.c` & `littlefs-python-0.6.2/littlefs/lfs_util.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/lfs_util.h` & `littlefs-python-0.6.2/littlefs/lfs_util.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/runners/bench_runner.c` & `littlefs-python-0.6.2/littlefs/runners/bench_runner.c`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/runners/bench_runner.h` & `littlefs-python-0.6.2/littlefs/runners/bench_runner.h`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/runners/test_runner.c` & `littlefs-python-0.6.2/littlefs/runners/test_runner.c`

 * *Files 2% similar despite different names*

```diff
@@ -1342,14 +1342,17 @@
         .read_size          = READ_SIZE,
         .prog_size          = PROG_SIZE,
         .block_size         = BLOCK_SIZE,
         .block_count        = BLOCK_COUNT,
         .block_cycles       = BLOCK_CYCLES,
         .cache_size         = CACHE_SIZE,
         .lookahead_size     = LOOKAHEAD_SIZE,
+    #ifdef LFS_MULTIVERSION
+        .disk_version       = DISK_VERSION,
+    #endif
     };
 
     struct lfs_emubd_config bdcfg = {
         .erase_value        = ERASE_VALUE,
         .erase_cycles       = ERASE_CYCLES,
         .badblock_behavior  = BADBLOCK_BEHAVIOR,
         .disk_path          = test_disk_path,
@@ -1411,14 +1414,17 @@
         .read_size          = READ_SIZE,
         .prog_size          = PROG_SIZE,
         .block_size         = BLOCK_SIZE,
         .block_count        = BLOCK_COUNT,
         .block_cycles       = BLOCK_CYCLES,
         .cache_size         = CACHE_SIZE,
         .lookahead_size     = LOOKAHEAD_SIZE,
+    #ifdef LFS_MULTIVERSION
+        .disk_version       = DISK_VERSION,
+    #endif
     };
 
     struct lfs_emubd_config bdcfg = {
         .erase_value        = ERASE_VALUE,
         .erase_cycles       = ERASE_CYCLES,
         .badblock_behavior  = BADBLOCK_BEHAVIOR,
         .disk_path          = test_disk_path,
@@ -1497,14 +1503,17 @@
         .read_size          = READ_SIZE,
         .prog_size          = PROG_SIZE,
         .block_size         = BLOCK_SIZE,
         .block_count        = BLOCK_COUNT,
         .block_cycles       = BLOCK_CYCLES,
         .cache_size         = CACHE_SIZE,
         .lookahead_size     = LOOKAHEAD_SIZE,
+    #ifdef LFS_MULTIVERSION
+        .disk_version       = DISK_VERSION,
+    #endif
     };
 
     struct lfs_emubd_config bdcfg = {
         .erase_value        = ERASE_VALUE,
         .erase_cycles       = ERASE_CYCLES,
         .badblock_behavior  = BADBLOCK_BEHAVIOR,
         .disk_path          = test_disk_path,
@@ -1581,14 +1590,17 @@
         .read_size          = READ_SIZE,
         .prog_size          = PROG_SIZE,
         .block_size         = BLOCK_SIZE,
         .block_count        = BLOCK_COUNT,
         .block_cycles       = BLOCK_CYCLES,
         .cache_size         = CACHE_SIZE,
         .lookahead_size     = LOOKAHEAD_SIZE,
+    #ifdef LFS_MULTIVERSION
+        .disk_version       = DISK_VERSION,
+    #endif
     };
 
     struct lfs_emubd_config bdcfg = {
         .erase_value        = ERASE_VALUE,
         .erase_cycles       = ERASE_CYCLES,
         .badblock_behavior  = BADBLOCK_BEHAVIOR,
         .disk_path          = test_disk_path,
@@ -1763,14 +1775,17 @@
         .read_size          = READ_SIZE,
         .prog_size          = PROG_SIZE,
         .block_size         = BLOCK_SIZE,
         .block_count        = BLOCK_COUNT,
         .block_cycles       = BLOCK_CYCLES,
         .cache_size         = CACHE_SIZE,
         .lookahead_size     = LOOKAHEAD_SIZE,
+    #ifdef LFS_MULTIVERSION
+        .disk_version       = DISK_VERSION,
+    #endif
     };
 
     struct lfs_emubd_config bdcfg = {
         .erase_value        = ERASE_VALUE,
         .erase_cycles       = ERASE_CYCLES,
         .badblock_behavior  = BADBLOCK_BEHAVIOR,
         .disk_path          = test_disk_path,
```

### Comparing `littlefs-python-0.5.0/littlefs/runners/test_runner.h` & `littlefs-python-0.6.2/littlefs/runners/test_runner.h`

 * *Files 4% similar despite different names*

```diff
@@ -87,38 +87,41 @@
 #define CACHE_SIZE_i         4
 #define LOOKAHEAD_SIZE_i     5
 #define BLOCK_CYCLES_i       6
 #define ERASE_VALUE_i        7
 #define ERASE_CYCLES_i       8
 #define BADBLOCK_BEHAVIOR_i  9
 #define POWERLOSS_BEHAVIOR_i 10
+#define DISK_VERSION_i       11
 
 #define READ_SIZE           TEST_DEFINE(READ_SIZE_i)
 #define PROG_SIZE           TEST_DEFINE(PROG_SIZE_i)
 #define BLOCK_SIZE          TEST_DEFINE(BLOCK_SIZE_i)
 #define BLOCK_COUNT         TEST_DEFINE(BLOCK_COUNT_i)
 #define CACHE_SIZE          TEST_DEFINE(CACHE_SIZE_i)
 #define LOOKAHEAD_SIZE      TEST_DEFINE(LOOKAHEAD_SIZE_i)
 #define BLOCK_CYCLES        TEST_DEFINE(BLOCK_CYCLES_i)
 #define ERASE_VALUE         TEST_DEFINE(ERASE_VALUE_i)
 #define ERASE_CYCLES        TEST_DEFINE(ERASE_CYCLES_i)
 #define BADBLOCK_BEHAVIOR   TEST_DEFINE(BADBLOCK_BEHAVIOR_i)
 #define POWERLOSS_BEHAVIOR  TEST_DEFINE(POWERLOSS_BEHAVIOR_i)
+#define DISK_VERSION        TEST_DEFINE(DISK_VERSION_i)
 
 #define TEST_IMPLICIT_DEFINES \
     TEST_DEF(READ_SIZE,          PROG_SIZE) \
     TEST_DEF(PROG_SIZE,          BLOCK_SIZE) \
     TEST_DEF(BLOCK_SIZE,         0) \
     TEST_DEF(BLOCK_COUNT,        (1024*1024)/BLOCK_SIZE) \
     TEST_DEF(CACHE_SIZE,         lfs_max(64,lfs_max(READ_SIZE,PROG_SIZE))) \
     TEST_DEF(LOOKAHEAD_SIZE,     16) \
     TEST_DEF(BLOCK_CYCLES,       -1) \
     TEST_DEF(ERASE_VALUE,        0xff) \
     TEST_DEF(ERASE_CYCLES,       0) \
     TEST_DEF(BADBLOCK_BEHAVIOR,  LFS_EMUBD_BADBLOCK_PROGERROR) \
-    TEST_DEF(POWERLOSS_BEHAVIOR, LFS_EMUBD_POWERLOSS_NOOP)
+    TEST_DEF(POWERLOSS_BEHAVIOR, LFS_EMUBD_POWERLOSS_NOOP) \
+    TEST_DEF(DISK_VERSION,       0)
 
-#define TEST_IMPLICIT_DEFINE_COUNT 11
+#define TEST_IMPLICIT_DEFINE_COUNT 12
 #define TEST_GEOMETRY_DEFINE_COUNT 4
 
 
 #endif
```

### Comparing `littlefs-python-0.5.0/littlefs/scripts/bench.py` & `littlefs-python-0.6.2/littlefs/scripts/bench.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/changeprefix.py` & `littlefs-python-0.6.2/littlefs/scripts/changeprefix.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/code.py` & `littlefs-python-0.6.2/littlefs/scripts/code.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/cov.py` & `littlefs-python-0.6.2/littlefs/scripts/cov.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/data.py` & `littlefs-python-0.6.2/littlefs/scripts/data.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/perf.py` & `littlefs-python-0.6.2/littlefs/scripts/perf.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/perfbd.py` & `littlefs-python-0.6.2/littlefs/scripts/perfbd.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/plot.py` & `littlefs-python-0.6.2/littlefs/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/plotmpl.py` & `littlefs-python-0.6.2/littlefs/scripts/plotmpl.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/prettyasserts.py` & `littlefs-python-0.6.2/littlefs/scripts/prettyasserts.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/readblock.py` & `littlefs-python-0.6.2/littlefs/scripts/readblock.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/readmdir.py` & `littlefs-python-0.6.2/littlefs/scripts/readmdir.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/readtree.py` & `littlefs-python-0.6.2/littlefs/scripts/readtree.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/stack.py` & `littlefs-python-0.6.2/littlefs/scripts/stack.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/structs.py` & `littlefs-python-0.6.2/littlefs/scripts/structs.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/summary.py` & `littlefs-python-0.6.2/littlefs/scripts/summary.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/tailpipe.py` & `littlefs-python-0.6.2/littlefs/scripts/tailpipe.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/teepipe.py` & `littlefs-python-0.6.2/littlefs/scripts/teepipe.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/test.py` & `littlefs-python-0.6.2/littlefs/scripts/test.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/tracebd.py` & `littlefs-python-0.6.2/littlefs/scripts/tracebd.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/scripts/watch.py` & `littlefs-python-0.6.2/littlefs/scripts/watch.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_alloc.toml` & `littlefs-python-0.6.2/littlefs/tests/test_alloc.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_attrs.toml` & `littlefs-python-0.6.2/littlefs/tests/test_attrs.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_badblocks.toml` & `littlefs-python-0.6.2/littlefs/tests/test_badblocks.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_bd.toml` & `littlefs-python-0.6.2/littlefs/tests/test_bd.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_compat.toml` & `littlefs-python-0.6.2/littlefs/tests/test_compat.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 # there may be a better way to do this, but oh well, explicit aliases works
 code = '''
 #ifdef LFSP
 #define STRINGIZE(x) STRINGIZE_(x)
 #define STRINGIZE_(x) #x
 #include STRINGIZE(LFSP)
 #else
-#define LFSP_VERSION LFS_VERSION
-#define LFSP_VERSION_MAJOR LFS_VERSION_MAJOR
-#define LFSP_VERSION_MINOR LFS_VERSION_MINOR
+#define LFSP_DISK_VERSION LFS_DISK_VERSION
+#define LFSP_DISK_VERSION_MAJOR LFS_DISK_VERSION_MAJOR
+#define LFSP_DISK_VERSION_MINOR LFS_DISK_VERSION_MINOR
 #define lfsp_t lfs_t
 #define lfsp_config lfs_config
 #define lfsp_format lfs_format
 #define lfsp_mount lfs_mount
 #define lfsp_unmount lfs_unmount
+#define lfsp_fsinfo lfs_fsinfo
+#define lfsp_fs_stat lfs_fs_stat
 #define lfsp_dir_t lfs_dir_t
 #define lfsp_info lfs_info
 #define LFSP_TYPE_REG LFS_TYPE_REG
 #define LFSP_TYPE_DIR LFS_TYPE_DIR
 #define lfsp_mkdir lfs_mkdir
 #define lfsp_dir_open lfs_dir_open
 #define lfsp_dir_read lfs_dir_read
@@ -54,15 +56,18 @@
 
 
 
 ## forward-compatibility tests ##
 
 # test we can mount in a new version
 [cases.test_compat_forward_mount]
-if = 'LFS_VERSION_MAJOR == LFSP_VERSION_MAJOR'
+if = '''
+    LFS_DISK_VERSION_MAJOR == LFSP_DISK_VERSION_MAJOR
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the previous version
     struct lfsp_config cfgp;
     memcpy(&cfgp, cfg, sizeof(cfgp));
     lfsp_t lfsp;
     lfsp_format(&lfsp, &cfgp) => 0;
 
@@ -70,21 +75,30 @@
     lfsp_mount(&lfsp, &cfgp) => 0;
     lfsp_unmount(&lfsp) => 0;
 
 
     // now test the new mount
     lfs_t lfs;
     lfs_mount(&lfs, cfg) => 0;
+
+    // we should be able to read the version using lfs_fs_stat
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFSP_DISK_VERSION);
+
     lfs_unmount(&lfs) => 0;
 '''
 
 # test we can read dirs in a new version
 [cases.test_compat_forward_read_dirs]
 defines.COUNT = 5
-if = 'LFS_VERSION_MAJOR == LFSP_VERSION_MAJOR'
+if = '''
+    LFS_DISK_VERSION_MAJOR == LFSP_DISK_VERSION_MAJOR
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the previous version
     struct lfsp_config cfgp;
     memcpy(&cfgp, cfg, sizeof(cfgp));
     lfsp_t lfsp;
     lfsp_format(&lfsp, &cfgp) => 0;
 
@@ -98,14 +112,19 @@
     lfsp_unmount(&lfsp) => 0;
 
 
     // mount the new version
     lfs_t lfs;
     lfs_mount(&lfs, cfg) => 0;
 
+    // we should be able to read the version using lfs_fs_stat
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFSP_DISK_VERSION);
+
     // can we list the directories?
     lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
@@ -128,15 +147,18 @@
 '''
 
 # test we can read files in a new version
 [cases.test_compat_forward_read_files]
 defines.COUNT = 5
 defines.SIZE = [4, 32, 512, 8192]
 defines.CHUNK = 4
-if = 'LFS_VERSION_MAJOR == LFSP_VERSION_MAJOR'
+if = '''
+    LFS_DISK_VERSION_MAJOR == LFSP_DISK_VERSION_MAJOR
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the previous version
     struct lfsp_config cfgp;
     memcpy(&cfgp, cfg, sizeof(cfgp));
     lfsp_t lfsp;
     lfsp_format(&lfsp, &cfgp) => 0;
 
@@ -162,14 +184,19 @@
     lfsp_unmount(&lfsp) => 0;
 
 
     // mount the new version
     lfs_t lfs;
     lfs_mount(&lfs, cfg) => 0;
 
+    // we should be able to read the version using lfs_fs_stat
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFSP_DISK_VERSION);
+
     // can we list the files?
     lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
@@ -210,15 +237,18 @@
 '''
 
 # test we can read files in dirs in a new version
 [cases.test_compat_forward_read_files_in_dirs]
 defines.COUNT = 5
 defines.SIZE = [4, 32, 512, 8192]
 defines.CHUNK = 4
-if = 'LFS_VERSION_MAJOR == LFSP_VERSION_MAJOR'
+if = '''
+    LFS_DISK_VERSION_MAJOR == LFSP_DISK_VERSION_MAJOR
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the previous version
     struct lfsp_config cfgp;
     memcpy(&cfgp, cfg, sizeof(cfgp));
     lfsp_t lfsp;
     lfsp_format(&lfsp, &cfgp) => 0;
 
@@ -247,14 +277,19 @@
     lfsp_unmount(&lfsp) => 0;
 
 
     // mount the new version
     lfs_t lfs;
     lfs_mount(&lfs, cfg) => 0;
 
+    // we should be able to read the version using lfs_fs_stat
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFSP_DISK_VERSION);
+
     // can we list the directories?
     lfs_dir_t dir;
     lfs_dir_open(&lfs, &dir, "/") => 0;
     struct lfs_info info;
     lfs_dir_read(&lfs, &dir, &info) => 1;
     assert(info.type == LFS_TYPE_DIR);
     assert(strcmp(info.name, ".") == 0);
@@ -317,15 +352,18 @@
 
     lfs_unmount(&lfs) => 0;
 '''
 
 # test we can write dirs in a new version
 [cases.test_compat_forward_write_dirs]
 defines.COUNT = 10
-if = 'LFS_VERSION_MAJOR == LFSP_VERSION_MAJOR'
+if = '''
+    LFS_DISK_VERSION_MAJOR == LFSP_DISK_VERSION_MAJOR
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the previous version
     struct lfsp_config cfgp;
     memcpy(&cfgp, cfg, sizeof(cfgp));
     lfsp_t lfsp;
     lfsp_format(&lfsp, &cfgp) => 0;
 
@@ -339,14 +377,19 @@
     lfsp_unmount(&lfsp) => 0;
 
 
     // mount the new version
     lfs_t lfs;
     lfs_mount(&lfs, cfg) => 0;
 
+    // we should be able to read the version using lfs_fs_stat
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFSP_DISK_VERSION);
+
     // write another COUNT/2 dirs
     for (lfs_size_t i = COUNT/2; i < COUNT; i++) {
         char name[8];
         sprintf(name, "dir%03d", i);
         lfs_mkdir(&lfs, name) => 0;
     }
 
@@ -376,15 +419,18 @@
 '''
 
 # test we can write files in a new version
 [cases.test_compat_forward_write_files]
 defines.COUNT = 5
 defines.SIZE = [4, 32, 512, 8192]
 defines.CHUNK = 2
-if = 'LFS_VERSION_MAJOR == LFSP_VERSION_MAJOR'
+if = '''
+    LFS_DISK_VERSION_MAJOR == LFSP_DISK_VERSION_MAJOR
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the previous version
     struct lfsp_config cfgp;
     memcpy(&cfgp, cfg, sizeof(cfgp));
     lfsp_t lfsp;
     lfsp_format(&lfsp, &cfgp) => 0;
 
@@ -416,14 +462,19 @@
     lfsp_unmount(&lfsp) => 0;
 
 
     // mount the new version
     lfs_t lfs;
     lfs_mount(&lfs, cfg) => 0;
 
+    // we should be able to read the version using lfs_fs_stat
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFSP_DISK_VERSION);
+
     // write half COUNT files
     prng = 42;
     for (lfs_size_t i = 0; i < COUNT; i++) {
         // skip half but keep our prng reproducible
         for (lfs_size_t j = 0; j < SIZE/2; j++) {
             TEST_PRNG(&prng);
         }
@@ -490,15 +541,18 @@
 '''
 
 # test we can write files in dirs in a new version
 [cases.test_compat_forward_write_files_in_dirs]
 defines.COUNT = 5
 defines.SIZE = [4, 32, 512, 8192]
 defines.CHUNK = 2
-if = 'LFS_VERSION_MAJOR == LFSP_VERSION_MAJOR'
+if = '''
+    LFS_DISK_VERSION_MAJOR == LFSP_DISK_VERSION_MAJOR
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the previous version
     struct lfsp_config cfgp;
     memcpy(&cfgp, cfg, sizeof(cfgp));
     lfsp_t lfsp;
     lfsp_format(&lfsp, &cfgp) => 0;
 
@@ -533,14 +587,19 @@
     lfsp_unmount(&lfsp) => 0;
 
 
     // mount the new version
     lfs_t lfs;
     lfs_mount(&lfs, cfg) => 0;
 
+    // we should be able to read the version using lfs_fs_stat
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFSP_DISK_VERSION);
+
     // write half COUNT files
     prng = 42;
     for (lfs_size_t i = 0; i < COUNT; i++) {
         // skip half but keep our prng reproducible
         for (lfs_size_t j = 0; j < SIZE/2; j++) {
             TEST_PRNG(&prng);
         }
@@ -632,36 +691,43 @@
 
 
 
 ## backwards-compatibility tests ##
 
 # test we can mount in an old version
 [cases.test_compat_backward_mount]
-if = 'LFS_VERSION == LFSP_VERSION'
+if = '''
+    LFS_DISK_VERSION == LFSP_DISK_VERSION
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the new version
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
 
     // confirm the new mount works
     lfs_mount(&lfs, cfg) => 0;
     lfs_unmount(&lfs) => 0;
 
     // now test the previous mount
     struct lfsp_config cfgp;
     memcpy(&cfgp, cfg, sizeof(cfgp));
     lfsp_t lfsp;
     lfsp_mount(&lfsp, &cfgp) => 0;
+
     lfsp_unmount(&lfsp) => 0;
 '''
 
 # test we can read dirs in an old version
 [cases.test_compat_backward_read_dirs]
 defines.COUNT = 5
-if = 'LFS_VERSION == LFSP_VERSION'
+if = '''
+    LFS_DISK_VERSION == LFSP_DISK_VERSION
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the new version
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
 
     // write COUNT dirs
     lfs_mount(&lfs, cfg) => 0;
@@ -705,15 +771,18 @@
 '''
 
 # test we can read files in an old version
 [cases.test_compat_backward_read_files]
 defines.COUNT = 5
 defines.SIZE = [4, 32, 512, 8192]
 defines.CHUNK = 4
-if = 'LFS_VERSION == LFSP_VERSION'
+if = '''
+    LFS_DISK_VERSION == LFSP_DISK_VERSION
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the new version
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
 
     // write COUNT files
     lfs_mount(&lfs, cfg) => 0;
@@ -787,15 +856,18 @@
 '''
 
 # test we can read files in dirs in an old version
 [cases.test_compat_backward_read_files_in_dirs]
 defines.COUNT = 5
 defines.SIZE = [4, 32, 512, 8192]
 defines.CHUNK = 4
-if = 'LFS_VERSION == LFSP_VERSION'
+if = '''
+    LFS_DISK_VERSION == LFSP_DISK_VERSION
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the new version
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
 
     // write COUNT files+dirs
     lfs_mount(&lfs, cfg) => 0;
@@ -894,15 +966,18 @@
 
     lfsp_unmount(&lfsp) => 0;
 '''
 
 # test we can write dirs in an old version
 [cases.test_compat_backward_write_dirs]
 defines.COUNT = 10
-if = 'LFS_VERSION == LFSP_VERSION'
+if = '''
+    LFS_DISK_VERSION == LFSP_DISK_VERSION
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the new version
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
 
     // write COUNT/2 dirs
     lfs_mount(&lfs, cfg) => 0;
@@ -953,15 +1028,18 @@
 '''
 
 # test we can write files in an old version
 [cases.test_compat_backward_write_files]
 defines.COUNT = 5
 defines.SIZE = [4, 32, 512, 8192]
 defines.CHUNK = 2
-if = 'LFS_VERSION == LFSP_VERSION'
+if = '''
+    LFS_DISK_VERSION == LFSP_DISK_VERSION
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the previous version
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
 
     // write half COUNT files
     lfs_mount(&lfs, cfg) => 0;
@@ -1067,15 +1145,18 @@
 '''
 
 # test we can write files in dirs in an old version
 [cases.test_compat_backward_write_files_in_dirs]
 defines.COUNT = 5
 defines.SIZE = [4, 32, 512, 8192]
 defines.CHUNK = 2
-if = 'LFS_VERSION == LFSP_VERSION'
+if = '''
+    LFS_DISK_VERSION == LFSP_DISK_VERSION
+        && DISK_VERSION == 0
+'''
 code = '''
     // create the previous version
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
 
     // write half COUNT files
     lfs_mount(&lfs, cfg) => 0;
@@ -1276,15 +1357,18 @@
     // mount should now fail
     lfs_mount(&lfs, cfg) => LFS_ERR_INVAL;
 '''
 
 # test that we correctly bump the minor version
 [cases.test_compat_minor_bump]
 in = 'lfs.c'
-if = 'LFS_DISK_VERSION_MINOR > 0'
+if = '''
+    LFS_DISK_VERSION_MINOR > 0
+        && DISK_VERSION == 0
+'''
 code = '''
     // create a superblock
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
     lfs_mount(&lfs, cfg) => 0;
     lfs_file_t file;
     lfs_file_open(&lfs, &file, "test",
@@ -1312,49 +1396,58 @@
     lfs_dir_commit(&lfs, &mdir, LFS_MKATTRS(
             {LFS_MKTAG(LFS_TYPE_INLINESTRUCT, 0, sizeof(superblock)),
                 &superblock})) => 0;
     lfs_unmount(&lfs) => 0;
 
     // mount should still work
     lfs_mount(&lfs, cfg) => 0;
+
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFS_DISK_VERSION-1);
+
     lfs_file_open(&lfs, &file, "test", LFS_O_RDONLY) => 0;
     uint8_t buffer[8];
     lfs_file_read(&lfs, &file, buffer, 8) => 8;
     assert(memcmp(buffer, "testtest", 8) == 0);
     lfs_file_close(&lfs, &file) => 0;
+
+    // minor version should be unchanged
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFS_DISK_VERSION-1);
+
     lfs_unmount(&lfs) => 0;
 
     // if we write, we need to bump the minor version
     lfs_mount(&lfs, cfg) => 0;
+
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFS_DISK_VERSION-1);
+
     lfs_file_open(&lfs, &file, "test", LFS_O_WRONLY | LFS_O_TRUNC) => 0;
     lfs_file_write(&lfs, &file, "teeeeest", 8) => 8;
     lfs_file_close(&lfs, &file) => 0;
 
-    // minor version should have changed
-    lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
-    lfs_dir_get(&lfs, &mdir, LFS_MKTAG(0x7ff, 0x3ff, 0),
-            LFS_MKTAG(LFS_TYPE_INLINESTRUCT, 0, sizeof(superblock)),
-            &superblock)
-            => LFS_MKTAG(LFS_TYPE_INLINESTRUCT, 0, sizeof(superblock));
-    lfs_superblock_fromle32(&superblock);
-    assert((superblock.version >> 16) & 0xffff == LFS_DISK_VERSION_MAJOR);
-    assert((superblock.version >>  0) & 0xffff == LFS_DISK_VERSION_MINOR);
+    // minor version should be changed
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFS_DISK_VERSION);
+
     lfs_unmount(&lfs) => 0;
 
     // and of course mount should still work
     lfs_mount(&lfs, cfg) => 0;
+
+    // minor version should have changed
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFS_DISK_VERSION);
+
     lfs_file_open(&lfs, &file, "test", LFS_O_RDONLY) => 0;
     lfs_file_read(&lfs, &file, buffer, 8) => 8;
     assert(memcmp(buffer, "teeeeest", 8) == 0);
     lfs_file_close(&lfs, &file) => 0;
 
-    // minor version should have changed
-    lfs_dir_fetch(&lfs, &mdir, (lfs_block_t[2]){0, 1}) => 0;
-    lfs_dir_get(&lfs, &mdir, LFS_MKTAG(0x7ff, 0x3ff, 0),
-            LFS_MKTAG(LFS_TYPE_INLINESTRUCT, 0, sizeof(superblock)),
-            &superblock)
-            => LFS_MKTAG(LFS_TYPE_INLINESTRUCT, 0, sizeof(superblock));
-    lfs_superblock_fromle32(&superblock);
-    assert((superblock.version >> 16) & 0xffff == LFS_DISK_VERSION_MAJOR);
-    assert((superblock.version >>  0) & 0xffff == LFS_DISK_VERSION_MINOR);
+    // yep, still changed
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFS_DISK_VERSION);
+
     lfs_unmount(&lfs) => 0;
 '''
```

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_dirs.toml` & `littlefs-python-0.6.2/littlefs/tests/test_dirs.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_entries.toml` & `littlefs-python-0.6.2/littlefs/tests/test_entries.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_evil.toml` & `littlefs-python-0.6.2/littlefs/tests/test_evil.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_exhaustion.toml` & `littlefs-python-0.6.2/littlefs/tests/test_exhaustion.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_files.toml` & `littlefs-python-0.6.2/littlefs/tests/test_files.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_interspersed.toml` & `littlefs-python-0.6.2/littlefs/tests/test_interspersed.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_move.toml` & `littlefs-python-0.6.2/littlefs/tests/test_move.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_orphans.toml` & `littlefs-python-0.6.2/littlefs/tests/test_orphans.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_paths.toml` & `littlefs-python-0.6.2/littlefs/tests/test_paths.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_powerloss.toml` & `littlefs-python-0.6.2/littlefs/tests/test_powerloss.toml`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,18 @@
     lfs_file_close(&lfs, &file) => 0;
 
     lfs_unmount(&lfs) => 0;
 '''
 
 # partial prog, may not be byte in order!
 [cases.test_powerloss_partial_prog]
-if = "PROG_SIZE < BLOCK_SIZE"
+if = '''
+    PROG_SIZE < BLOCK_SIZE
+        && (DISK_VERSION == 0 || DISK_VERSION >= 0x00020001)
+'''
 defines.BYTE_OFF = ["0", "PROG_SIZE-1", "PROG_SIZE/2"]
 defines.BYTE_VALUE = [0x33, 0xcc]
 in = "lfs.c"
 code = '''
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
```

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_relocations.toml` & `littlefs-python-0.6.2/littlefs/tests/test_relocations.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_seek.toml` & `littlefs-python-0.6.2/littlefs/tests/test_seek.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_superblocks.toml` & `littlefs-python-0.6.2/littlefs/tests/test_superblocks.toml`

 * *Files 24% similar despite different names*

```diff
@@ -30,14 +30,62 @@
 # invalid mount
 [cases.test_superblocks_invalid_mount]
 code = '''
     lfs_t lfs;
     lfs_mount(&lfs, cfg) => LFS_ERR_CORRUPT;
 '''
 
+# test we can read superblock info through lfs_fs_stat
+[cases.test_superblocks_stat]
+if = 'DISK_VERSION == 0'
+code = '''
+    lfs_t lfs;
+    lfs_format(&lfs, cfg) => 0;
+
+    // test we can mount and read fsinfo
+    lfs_mount(&lfs, cfg) => 0;
+
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFS_DISK_VERSION);
+    assert(fsinfo.name_max == LFS_NAME_MAX);
+    assert(fsinfo.file_max == LFS_FILE_MAX);
+    assert(fsinfo.attr_max == LFS_ATTR_MAX);
+
+    lfs_unmount(&lfs) => 0;
+'''
+
+[cases.test_superblocks_stat_tweaked]
+if = 'DISK_VERSION == 0'
+defines.TWEAKED_NAME_MAX = 63
+defines.TWEAKED_FILE_MAX = '(1 << 16)-1'
+defines.TWEAKED_ATTR_MAX = 512
+code = '''
+    // create filesystem with tweaked params
+    struct lfs_config tweaked_cfg = *cfg;
+    tweaked_cfg.name_max = TWEAKED_NAME_MAX;
+    tweaked_cfg.file_max = TWEAKED_FILE_MAX;
+    tweaked_cfg.attr_max = TWEAKED_ATTR_MAX;
+
+    lfs_t lfs;
+    lfs_format(&lfs, &tweaked_cfg) => 0;
+
+    // test we can mount and read these params with the original config
+    lfs_mount(&lfs, cfg) => 0;
+
+    struct lfs_fsinfo fsinfo;
+    lfs_fs_stat(&lfs, &fsinfo) => 0;
+    assert(fsinfo.disk_version == LFS_DISK_VERSION);
+    assert(fsinfo.name_max == TWEAKED_NAME_MAX);
+    assert(fsinfo.file_max == TWEAKED_FILE_MAX);
+    assert(fsinfo.attr_max == TWEAKED_ATTR_MAX);
+
+    lfs_unmount(&lfs) => 0;
+'''
+
 # expanding superblock
 [cases.test_superblocks_expand]
 defines.BLOCK_CYCLES = [32, 33, 1]
 defines.N = [10, 100, 1000]
 code = '''
     lfs_t lfs;
     lfs_format(&lfs, cfg) => 0;
```

### Comparing `littlefs-python-0.5.0/littlefs/tests/test_truncate.toml` & `littlefs-python-0.6.2/littlefs/tests/test_truncate.toml`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/setup.py` & `littlefs-python-0.6.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 EXTENSIONS = [
     Extension("littlefs.lfs", ["src/littlefs/lfs.pyx", 'littlefs/lfs.c', 'littlefs/lfs_util.c'],
               include_dirs=['littlefs'],
               define_macros=[
                   ('LFS_NO_DEBUG', '1'),
                   ('LFS_NO_WARN', '1'),
                   ('LFS_NO_ERROR', '1'),
+                  ('LFS_MULTIVERSION', '1'),
                 # ('LFS_YES_TRACE', '1')
               ],
               extra_compile_args=['-std=c99']
     )
 ]
 
 
@@ -43,13 +44,18 @@
     zip_safe=False,
     ext_modules=cythonize(EXTENSIONS, language_level=3, annotate=False,
                           compiler_directives={'embedsignature': True}),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development :: Embedded Systems',
         'Topic :: Software Development :: Libraries',
         'Topic :: System :: Filesystems'
     ]
 )
```

### Comparing `littlefs-python-0.5.0/src/littlefs/__init__.py` & `littlefs-python-0.6.2/src/littlefs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 import warnings
-from typing import TYPE_CHECKING, List, Tuple, Iterator, IO
+from typing import TYPE_CHECKING, List, Tuple, Iterator, IO, Union
 
 from pkg_resources import DistributionNotFound, get_distribution
 
 from . import errors, lfs
 from .lfs import __LFS_DISK_VERSION__, __LFS_VERSION__
 from .errors import LittleFSError
 
@@ -43,14 +43,22 @@
         """Format the underlying buffer"""
         return lfs.format(self.fs, self.cfg)
 
     def mount(self) -> int:
         """Mount the underlying buffer"""
         return lfs.mount(self.fs, self.cfg)
 
+    def fs_mkconsistent(self) -> int:
+        """Attempt to make the filesystem consistent and ready for writing"""
+        return lfs.fs_mkconsistent(self.fs)
+
+    def fs_stat(self) -> 'LFSFSStat':
+        """Get the status of the filesystem"""
+        return lfs.fs_stat(self.fs)
+
     def open(
         self,
         fname: str,
         mode='r',
         buffering: int = -1,
         encoding: str = None,
         errors: str = None,
@@ -191,14 +199,26 @@
             errors,
             newline,
             line_buffering
         )
 
         return wrapped
 
+    def getattr(self, path: str, typ: Union[str, bytes, int]) -> bytes:
+        typ = _typ_to_uint8(typ)
+        return lfs.getattr(self.fs, path, typ)
+
+    def setattr(self, path: str, typ: Union[str, bytes, int], data: bytes) -> None:
+        typ = _typ_to_uint8(typ)
+        lfs.setattr(self.fs, path, typ, data)
+
+    def removeattr(self, path: str, typ: Union[str, bytes, int]) -> None:
+        typ = _typ_to_uint8(typ)
+        lfs.removeattr(self.fs, path, typ)
+
     def listdir(self, path='.') -> List[str]:
         """List directory content
 
         List the content of a directory. This function uses :meth:`scandir`
         internally. Using :meth:`scandir` might be better if you are
         searching for a specific file or need access to the :class:`littlefs.lfs.LFSStat`
         of the files.
@@ -403,7 +423,18 @@
         size = file_size - file_pos
 
         return lfs.file_read(self.fs, self.fh, size)
 
     def flush(self):
         super().flush()
         lfs.file_sync(self.fs, self.fh)
+
+def _typ_to_uint8(typ):
+    try:
+        out = ord(typ)
+    except TypeError:
+        out = int(typ)
+
+    if not(0 <= out <= 255):
+        raise ValueError(f"type must be in range [0, 255]")
+
+    return out
```

### Comparing `littlefs-python-0.5.0/src/littlefs/context.py` & `littlefs-python-0.6.2/src/littlefs/context.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/src/littlefs/errors.py` & `littlefs-python-0.6.2/src/littlefs/errors.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/src/littlefs/lfs.pxd` & `littlefs-python-0.6.2/src/littlefs/lfs.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
     cdef const int LFS_DISK_VERSION
     cdef const int LFS_DISK_VERSION_MAJOR
     cdef const int LFS_DISK_VERSION_MINOR
 
     cdef const int LFS_NAME_MAX
 
+    cdef const int LFS_ATTR_MAX
+
 
     # Basic type definitions
     ctypedef uint32_t lfs_size_t
     ctypedef uint32_t lfs_off_t
 
     ctypedef int32_t  lfs_ssize_t
     ctypedef int32_t  lfs_soff_t
@@ -60,14 +62,20 @@
     ctypedef lfs lfs_t
 
     cdef struct lfs_info:
         uint8_t type
         lfs_size_t size
         char name[LFS_NAME_MAX+1]
 
+    cdef struct lfs_fsinfo:
+        uint32_t disk_version
+        lfs_size_t name_max
+        lfs_size_t file_max
+        lfs_size_t attr_max
+
     cdef struct lfs_dir:
         pass
 
     ctypedef lfs_dir lfs_dir_t
 
     cdef struct lfs_file:
         uint32_t flags
@@ -98,14 +106,16 @@
         lfs_size_t lookahead_size
         void *read_buffer
         void *prog_buffer
         void *lookahead_buffer
         lfs_size_t name_max
         lfs_size_t file_max
         lfs_size_t attr_max
+        lfs_size_t metadata_max
+        uint32_t disk_version
 
     int lfs_mount(lfs_t *lfs, const lfs_config *config)
     int lfs_format(lfs_t *lfs, const lfs_config *config)
     int lfs_unmount(lfs_t *lfs)
 
     int lfs_remove(lfs_t *lfs, const char *path)
     int lfs_rename(lfs_t *lfs, const char *oldpath, const char *newpath)
@@ -143,9 +153,11 @@
     int lfs_mkdir(lfs_t *lfs, const char *path)
     int lfs_dir_open(lfs_t *lfs, lfs_dir *dir, const char *path)
     int lfs_dir_close(lfs_t *lfs, lfs_dir *dir)
     int lfs_dir_read(lfs_t *lfs, lfs_dir *dir,  lfs_info *info)
     int lfs_dir_seek(lfs_t *lfs, lfs_dir *dir, lfs_off_t off)
     lfs_soff_t lfs_dir_tell(lfs_t *lfs, lfs_dir *dir)
     int lfs_dir_rewind(lfs_t *lfs, lfs_dir *dir)
+    int lfs_fs_stat(lfs_t *lfs, lfs_fsinfo* info)
     lfs_ssize_t lfs_fs_size(lfs_t *lfs)
     int lfs_fs_traverse(lfs_t *lfs, int (*cb)(void*, lfs_block_t), void *data)
+    int lfs_fs_mkconsistent(lfs_t *lfs)
```

### Comparing `littlefs-python-0.5.0/src/littlefs/lfs.pyi` & `littlefs-python-0.6.2/src/littlefs/lfs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,27 +49,29 @@
 
 # The following classes are opaque wrappers around the actual handles
 class LFSFilesystem: ...
 class LFSFile: ...
 class LFSDirectory: ...
 
 
+def fs_stat(fs: LFSFilesystem) -> LFSFSStat: ...
 def fs_size(fs: LFSFilesystem) -> int: ...
 def format(fs: LFSFilesystem, cfg: LFSConfig) -> int: ...
 def mount(fs: LFSFilesystem, cfg: LFSConfig) -> int: ...
 def unmount(fs: LFSFilesystem) -> int: ...
+def fs_mkconsistent(fs: LFSFilesystem) -> int: ...
 
 def remove(fs: LFSFilesystem, path: str) -> int: ...
 def rename(fs: LFSFilesystem, oldpath: str, newpath: str) -> int: ...
 def stat(fs: LFSFilesystem, path: str) -> LFSStat: ...
 
 # Attributes
-def getattr(fs: LFSFilesystem, path: str, type, buffer, size) -> int: ...
-def setattr(fs: LFSFilesystem, path: str, type, buffer, size) -> int: ...
-def removeattr(fs: LFSFilesystem, path: str, type) -> int: ...
+def getattr(fs: LFSFilesystem, path: str, typ) -> bytes: ...
+def setattr(fs: LFSFilesystem, path: str, typ, data) -> None: ...
+def removeattr(fs: LFSFilesystem, path: str, typ) -> None: ...
 
 # File Handling
 def file_open(fs: LFSFilesystem, path: str, flags: Union[str, LFSFileFlag]) -> LFSFile: ...
 # def file_open_cfg(self, path, flags, config): ...
 def file_close(fs: LFSFilesystem, fh: LFSFile) -> int: ...
 def file_sync(fs: LFSFilesystem, fh: LFSFile) -> int: ...
 def file_read(fs: LFSFilesystem, fh: LFSFile, size) -> bytes: ...
```

### Comparing `littlefs-python-0.5.0/src/littlefs/lfs.pyx` & `littlefs-python-0.6.2/src/littlefs/lfs.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 """Default filename encoding"""
 
 LFSStat = namedtuple('LFSStat', ['type', 'size', 'name'])
 LFSStat.__doc__ = """\
 Littlefs File / Directory status
 """
 
+LFSFSStat = namedtuple('LFSFSStat', ['disk_version', 'name_max', 'file_max', 'attr_max'])
+LFSFSStat.__doc__ = """\
+Littlefs filesystem status
+"""
+
 
 class LFSFileFlag(enum.IntFlag):
     """Littlefs file mode flags"""
     rdonly = LFS_O_RDONLY
     wronly = LFS_O_WRONLY
     rdwr = LFS_O_RDWR
     creat = LFS_O_CREAT
@@ -29,33 +34,33 @@
 
 
 # Export LFS version and disk version to python
 __LFS_VERSION__ = (LFS_VERSION_MAJOR, LFS_VERSION_MINOR)
 __LFS_DISK_VERSION__ = (LFS_DISK_VERSION_MAJOR, LFS_DISK_VERSION_MINOR)
 
 
-cdef int _lfs_read(const lfs_config *c, lfs_block_t block, lfs_off_t off, void * buffer, lfs_size_t size):
+cdef int _lfs_read(const lfs_config *c, lfs_block_t block, lfs_off_t off, void * buffer, lfs_size_t size) noexcept:
     ctx = <object>c.context
     data = ctx.user_context.read(ctx, block, off, size)
     memcpy(buffer, <char *>data, size)
     return 0
 
 
-cdef int _lfs_prog(const lfs_config *c, lfs_block_t block, lfs_off_t off, const void * buffer, lfs_size_t size):
+cdef int _lfs_prog(const lfs_config *c, lfs_block_t block, lfs_off_t off, const void * buffer, lfs_size_t size) noexcept:
     ctx = <object>c.context
     data = (<char*>buffer)[:size]
     return ctx.user_context.prog(ctx, block, off, data)
 
 
-cdef int _lfs_erase(const lfs_config *c, lfs_block_t block):
+cdef int _lfs_erase(const lfs_config *c, lfs_block_t block) noexcept:
     ctx = <object>c.context
     return ctx.user_context.erase(ctx, block)
 
 
-cdef int _lfs_sync(const lfs_config *c):
+cdef int _lfs_sync(const lfs_config *c) noexcept:
     ctx = <object>c.context
     return ctx.user_context.sync(ctx)
 
 
 cdef int _raise_on_error(int code) except -1:
     if code < 0:
         raise errors.LittleFSError(code)
@@ -92,14 +97,16 @@
         # Cache size, at least as big as read / prog size
         self._impl.cache_size = kwargs.get('cache_size', max(self._impl.read_size, self._impl.prog_size))
         # Lookahead buffer size in bytes
         self._impl.lookahead_size = kwargs.get('lookahead_size', 8)
         self._impl.name_max = kwargs.get('name_max', 0)
         self._impl.file_max = kwargs.get('file_max', 0)
         self._impl.attr_max = kwargs.get('attr_max', 0)
+        self._impl.metadata_max = kwargs.get('metadata_max', 0)
+        self._impl.disk_version = kwargs.get('disk_version', 0)
 
         if context is None:
             context = UserContext(self._impl.block_size * self._impl.block_count)
 
         self.user_context = context
         self._impl.context = <void *>self
 
@@ -135,14 +142,22 @@
     def file_max(self):
         return self._impl.file_max
 
     @property
     def attr_max(self):
         return self._impl.attr_max
 
+    @property
+    def metadata_max(self):
+        return self._impl.metadata_max
+
+    @property
+    def disk_version(self):
+        return self._impl.disk_version
+
 
 cdef class LFSFilesystem:
     cdef lfs_t _impl
 
 
 cdef class LFSFile:
     cdef lfs_file_t _impl
@@ -153,14 +168,24 @@
         return LFSFileFlag(self._impl.flags)
 
 
 cdef class LFSDirectory:
     cdef lfs_dir_t _impl
 
 
+def fs_stat(LFSFilesystem fs):
+    """Get filesystem status"""
+    cdef lfs_fsinfo * info = <lfs_fsinfo *>malloc(sizeof(lfs_fsinfo))
+    try:
+        _raise_on_error(lfs_fs_stat(&fs._impl, info))
+        return LFSFSStat(info.disk_version, info.name_max, info.file_max, info.attr_max)
+    finally:
+        free(info)
+
+
 def fs_size(LFSFilesystem fs):
     return _raise_on_error(lfs_fs_size(&fs._impl))
 
 
 def format(LFSFilesystem fs, LFSConfig cfg):
     """Format the filesystem"""
     return _raise_on_error(lfs_format(&fs._impl, &cfg._impl))
@@ -175,14 +200,19 @@
     """Unmount the filesystem
 
     This does nothing beside releasing any allocated resources
     """
     return _raise_on_error(lfs_unmount(&fs._impl))
 
 
+def fs_mkconsistent(LFSFilesystem fs):
+    """Attempt to make the filesystem consistent and ready for writing"""
+    return _raise_on_error(lfs_fs_mkconsistent(&fs._impl))
+
+
 def remove(LFSFilesystem fs, path):
     """Remove a file or directory
 
     If removing a direcotry, the directory must be empty.
     """
     return _raise_on_error(lfs_remove(&fs._impl, path.encode(FILENAME_ENCODING)))
 
@@ -202,24 +232,28 @@
     try:
         _raise_on_error(lfs_stat(&fs._impl, path.encode(FILENAME_ENCODING), info))
         return LFSStat(info.type, info.size, info.name.decode(FILENAME_ENCODING))
     finally:
         free(info)
 
 
-def getattr(LFSFilesystem fs, path, type, buffer, size):
-    raise NotImplementedError
+def getattr(LFSFilesystem fs, path, typ):
+    buf = bytearray(LFS_ATTR_MAX)
+    cdef unsigned char[::1] buf_view = buf
+    attr_size = _raise_on_error(lfs_getattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], LFS_ATTR_MAX))
+    return bytes(buf[:attr_size])
 
 
-def setattr(LFSFilesystem fs, path, type, buffer, size):
-    raise NotImplementedError
+def setattr(LFSFilesystem fs, path, typ, data):
+    cdef const unsigned char[::1] buf_view = data
+    _raise_on_error(lfs_setattr(&fs._impl, path.encode(FILENAME_ENCODING), typ, &buf_view[0], len(data)))
 
 
-def removeattr(LFSFilesystem fs, path, type):
-    raise NotImplementedError
+def removeattr(LFSFilesystem fs, path, typ):
+    _raise_on_error(lfs_removeattr(&fs._impl, path.encode(FILENAME_ENCODING), typ))
 
 
 def file_open(LFSFilesystem fs, path, flags):
     if isinstance(flags, str):
         creating = False
         reading = False
         writing = False
```

### Comparing `littlefs-python-0.5.0/src/littlefs_python.egg-info/PKG-INFO` & `littlefs-python-0.6.2/src/littlefs_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: littlefs-python
-Version: 0.5.0
+Version: 0.6.2
 Summary: A python wrapper for littlefs
 Home-page: https://github.com/jrast/littlefs-python
 Author: Jürg Rast
 Author-email: juergr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -86,28 +91,32 @@
     As littlefs_ is bundled with the package you will need to install the correct version of
     this package in successfully read or create images for your embedded system. If you start
     from scratch the latest version is recommeded.
 
     .. csv-table::
         :header: "Package Version", "LittleFS Version", "LittleFS File System Version"
 
-        0.6.0, 2.6.1, 2.1
-        0.5.0, 2.4.1, 2.0
+        0.6.0, 2.7.0, 2.0 / 2.1 [#f1]_
+        0.5.0, 2.6.1, 2.1
         0.4.0, 2.2.1, 2.0
+        0.3.0, 2.2.1, 2.0
+
+    .. [#f1] See ``test/test_multiversion.py`` for examples.
 
 
 This is as simple as it can be::
 
     pip install littlefs-python
 
 At the moment wheels (which require no build) are provided for the following platforms,
 on other platforms the source package is used and a compiler is required:
 
- - Linux: Python 3.6 - 3.10 / 32- & 64-bit
- - Windows: Python 3.6 - 3.10 / 32- & 64-bit
+ - Linux: Python 3.6 - 3.11 / x86_64, arm64
+ - MacOS: Python 3.6 - 3.11 / x86_64, arm64
+ - Windows: Python 3.6 - 3.11 / 32- & 64-bit
 
 
 Development Setup
 =================
 
 Start by checking out the source repository of littlefs-python::
```

### Comparing `littlefs-python-0.5.0/src/littlefs_python.egg-info/SOURCES.txt` & `littlefs-python-0.6.2/src/littlefs_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -101,16 +101,18 @@
 src/littlefs/lfs.pyx
 src/littlefs/py.typed
 src/littlefs_python.egg-info/PKG-INFO
 src/littlefs_python.egg-info/SOURCES.txt
 src/littlefs_python.egg-info/dependency_links.txt
 src/littlefs_python.egg-info/not-zip-safe
 src/littlefs_python.egg-info/top_level.txt
+test/test_attr.py
 test/test_directories.py
 test/test_files.py
+test/test_multiversion.py
 test/test_remove_rename.py
 test/test_version.py
 test/test_walk.py
 test/lfs/conftest.py
 test/lfs/test_dir_functions.py
 test/lfs/test_file_functions.py
 test/lfs/test_fs_functions.py
```

### Comparing `littlefs-python-0.5.0/test/lfs/conftest.py` & `littlefs-python-0.6.2/test/lfs/conftest.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/test/lfs/test_dir_functions.py` & `littlefs-python-0.6.2/test/lfs/test_dir_functions.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/test/lfs/test_file_functions.py` & `littlefs-python-0.6.2/test/lfs/test_file_functions.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/test/lfs/test_fs_functions.py` & `littlefs-python-0.6.2/test/lfs/test_fs_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,7 +42,17 @@
     lfs.file_close(mounted_fs, fh)
 
     stat = lfs.stat(mounted_fs, 'test.txt')
 
     assert stat.size == 10
     assert stat.type == 1
     assert stat.name == 'test.txt'
+
+
+def test_fs_stat(mounted_fs):
+    """Test if fs stat works"""
+    stat = lfs.fs_stat(mounted_fs)
+    # The following values are defaults in littlefs.
+    assert stat.disk_version == 0x00020001
+    assert stat.name_max == 255
+    assert stat.file_max == 2147483647
+    assert stat.attr_max == 1022
```

### Comparing `littlefs-python-0.5.0/test/test_directories.py` & `littlefs-python-0.6.2/test/test_directories.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/test/test_files.py` & `littlefs-python-0.6.2/test/test_files.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/test/test_remove_rename.py` & `littlefs-python-0.6.2/test/test_remove_rename.py`

 * *Files identical despite different names*

### Comparing `littlefs-python-0.5.0/test/test_walk.py` & `littlefs-python-0.6.2/test/test_walk.py`

 * *Files identical despite different names*

