# Comparing `tmp/clr_loader-0.2.5.tar.gz` & `tmp/clr_loader-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clr_loader-0.2.5.tar", last modified: Tue Jan  3 12:18:15 2023, max compression
+gzip compressed data, was "clr_loader-0.2.6.tar", last modified: Mon Aug  7 15:22:57 2023, max compression
```

## Comparing `clr_loader-0.2.5.tar` & `clr_loader-0.2.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.480144 clr_loader-0.2.5/
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.466811 clr_loader-0.2.5/.github/
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.470144 clr_loader-0.2.5/.github/workflows/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      742 2023-01-03 12:09:35.000000 clr_loader-0.2.5/.github/workflows/ci-arm.yml
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     2648 2023-01-03 12:09:35.000000 clr_loader-0.2.5/.github/workflows/ci.yml
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      851 2022-09-23 05:27:39.000000 clr_loader-0.2.5/.github/workflows/docs.yml
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      796 2019-11-06 09:17:45.000000 clr_loader-0.2.5/.gitignore
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.470144 clr_loader-0.2.5/.vscode/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      229 2022-01-15 11:18:11.000000 clr_loader-0.2.5/.vscode/launch.json
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1079 2022-03-10 15:56:45.000000 clr_loader-0.2.5/LICENSE
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      111 2019-11-07 08:00:09.000000 clr_loader-0.2.5/MANIFEST.in
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1396 2023-01-03 12:18:15.480144 clr_loader-0.2.5/PKG-INFO
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      673 2022-09-16 21:09:21.000000 clr_loader-0.2.5/README.md
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.470144 clr_loader-0.2.5/clr_loader/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     5982 2023-01-03 12:15:46.000000 clr_loader-0.2.5/clr_loader/__init__.py
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.473477 clr_loader-0.2.5/clr_loader/ffi/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     2131 2022-10-14 13:45:50.000000 clr_loader-0.2.5/clr_loader/ffi/__init__.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     3083 2022-09-16 18:54:33.000000 clr_loader-0.2.5/clr_loader/ffi/hostfxr.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1501 2023-01-03 12:15:46.000000 clr_loader-0.2.5/clr_loader/ffi/mono.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      420 2021-02-13 17:01:41.000000 clr_loader-0.2.5/clr_loader/ffi/netfx.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     5064 2022-10-13 10:34:23.000000 clr_loader-0.2.5/clr_loader/hostfxr.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     6267 2023-01-03 12:15:46.000000 clr_loader-0.2.5/clr_loader/mono.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1631 2023-01-03 12:15:39.000000 clr_loader-0.2.5/clr_loader/netfx.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     4643 2022-09-16 19:02:54.000000 clr_loader-0.2.5/clr_loader/types.py
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.476811 clr_loader-0.2.5/clr_loader/util/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1028 2022-09-16 18:54:33.000000 clr_loader-0.2.5/clr_loader/util/__init__.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      712 2021-02-13 17:33:47.000000 clr_loader-0.2.5/clr_loader/util/clr_error.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)    80037 2020-12-12 21:49:19.000000 clr_loader-0.2.5/clr_loader/util/coreclr_errors.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     4804 2023-01-03 12:15:46.000000 clr_loader-0.2.5/clr_loader/util/find.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1937 2020-12-12 21:49:19.000000 clr_loader-0.2.5/clr_loader/util/hostfxr_errors.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      766 2022-09-16 19:02:54.000000 clr_loader-0.2.5/clr_loader/util/runtime_spec.py
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.473477 clr_loader-0.2.5/clr_loader.egg-info/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1396 2023-01-03 12:18:15.000000 clr_loader-0.2.5/clr_loader.egg-info/PKG-INFO
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1067 2023-01-03 12:18:15.000000 clr_loader-0.2.5/clr_loader.egg-info/SOURCES.txt
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)        1 2023-01-03 12:18:15.000000 clr_loader-0.2.5/clr_loader.egg-info/dependency_links.txt
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)        1 2023-01-03 12:00:14.000000 clr_loader-0.2.5/clr_loader.egg-info/not-zip-safe
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)       11 2023-01-03 12:18:15.000000 clr_loader-0.2.5/clr_loader.egg-info/requires.txt
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)       11 2023-01-03 12:18:15.000000 clr_loader-0.2.5/clr_loader.egg-info/top_level.txt
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.476811 clr_loader-0.2.5/doc/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)        8 2022-09-16 19:02:54.000000 clr_loader-0.2.5/doc/.gitignore
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      634 2022-09-16 19:02:54.000000 clr_loader-0.2.5/doc/Makefile
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      643 2022-10-15 07:15:18.000000 clr_loader-0.2.5/doc/conf.py
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      953 2022-09-16 19:02:54.000000 clr_loader-0.2.5/doc/index.rst
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      800 2022-09-16 19:02:54.000000 clr_loader-0.2.5/doc/make.bat
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      502 2022-09-16 19:02:54.000000 clr_loader-0.2.5/doc/reference.rst
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)       69 2022-09-23 05:27:39.000000 clr_loader-0.2.5/doc/requirements.txt
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     3350 2022-09-17 07:04:41.000000 clr_loader-0.2.5/doc/usage.rst
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.480144 clr_loader-0.2.5/example/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      631 2019-10-31 07:39:07.000000 clr_loader-0.2.5/example/TestClass.cs
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      526 2022-07-07 23:21:50.000000 clr_loader-0.2.5/example/example.csproj
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1720 2019-10-23 09:00:44.000000 clr_loader-0.2.5/example/example.sln
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.480144 clr_loader-0.2.5/netfx_loader/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     3383 2023-01-03 12:15:39.000000 clr_loader-0.2.5/netfx_loader/ClrLoader.cs
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)      838 2020-12-12 21:49:19.000000 clr_loader-0.2.5/netfx_loader/ClrLoader.csproj
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1777 2019-11-07 06:35:11.000000 clr_loader-0.2.5/netfx_loader/ClrLoader.sln
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1628 2021-02-13 17:01:41.000000 clr_loader-0.2.5/netfx_loader/DomainData.cs
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1203 2022-10-15 07:15:28.000000 clr_loader-0.2.5/pyproject.toml
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)       38 2023-01-03 12:18:15.480144 clr_loader-0.2.5/setup.cfg
--rwxr-xr-x   0 benedikt  (1000) benedikt  (1000)     4071 2022-10-15 07:15:18.000000 clr_loader-0.2.5/setup.py
-drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-01-03 12:18:15.480144 clr_loader-0.2.5/tests/
--rw-r--r--   0 benedikt  (1000) benedikt  (1000)     2819 2023-01-03 12:15:46.000000 clr_loader-0.2.5/tests/test_common.py
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:57.006337 clr_loader-0.2.6/
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:56.986337 clr_loader-0.2.6/.github/
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:56.989670 clr_loader-0.2.6/.github/workflows/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      742 2023-01-03 12:09:35.000000 clr_loader-0.2.6/.github/workflows/ci-arm.yml
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     2649 2023-08-07 13:24:35.000000 clr_loader-0.2.6/.github/workflows/ci.yml
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      851 2022-09-23 05:27:39.000000 clr_loader-0.2.6/.github/workflows/docs.yml
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      796 2019-11-06 09:17:45.000000 clr_loader-0.2.6/.gitignore
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:56.993004 clr_loader-0.2.6/.vscode/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      229 2022-01-15 11:18:11.000000 clr_loader-0.2.6/.vscode/launch.json
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1079 2022-03-10 15:56:45.000000 clr_loader-0.2.6/LICENSE
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      111 2019-11-07 08:00:09.000000 clr_loader-0.2.6/MANIFEST.in
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1396 2023-08-07 15:22:57.006337 clr_loader-0.2.6/PKG-INFO
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      673 2022-09-16 21:09:21.000000 clr_loader-0.2.6/README.md
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:56.993004 clr_loader-0.2.6/clr_loader/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     6009 2023-08-07 13:26:00.000000 clr_loader-0.2.6/clr_loader/__init__.py
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:56.996337 clr_loader-0.2.6/clr_loader/ffi/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     2131 2022-10-14 13:45:50.000000 clr_loader-0.2.6/clr_loader/ffi/__init__.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     3083 2022-09-16 18:54:33.000000 clr_loader-0.2.6/clr_loader/ffi/hostfxr.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1501 2023-01-05 18:39:19.000000 clr_loader-0.2.6/clr_loader/ffi/mono.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      420 2021-02-13 17:01:41.000000 clr_loader-0.2.6/clr_loader/ffi/netfx.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     4907 2023-08-07 15:21:26.000000 clr_loader-0.2.6/clr_loader/hostfxr.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     6297 2023-08-07 13:24:35.000000 clr_loader-0.2.6/clr_loader/mono.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1858 2023-08-07 15:21:26.000000 clr_loader-0.2.6/clr_loader/netfx.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     4643 2022-09-16 19:02:54.000000 clr_loader-0.2.6/clr_loader/types.py
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:56.999671 clr_loader-0.2.6/clr_loader/util/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1028 2022-09-16 18:54:33.000000 clr_loader-0.2.6/clr_loader/util/__init__.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      712 2021-02-13 17:33:47.000000 clr_loader-0.2.6/clr_loader/util/clr_error.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)    80037 2020-12-12 21:49:19.000000 clr_loader-0.2.6/clr_loader/util/coreclr_errors.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     4988 2023-08-07 13:26:04.000000 clr_loader-0.2.6/clr_loader/util/find.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1937 2020-12-12 21:49:19.000000 clr_loader-0.2.6/clr_loader/util/hostfxr_errors.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      766 2022-09-16 19:02:54.000000 clr_loader-0.2.6/clr_loader/util/runtime_spec.py
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:56.996337 clr_loader-0.2.6/clr_loader.egg-info/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1396 2023-08-07 15:22:56.000000 clr_loader-0.2.6/clr_loader.egg-info/PKG-INFO
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1067 2023-08-07 15:22:56.000000 clr_loader-0.2.6/clr_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)        1 2023-08-07 15:22:56.000000 clr_loader-0.2.6/clr_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)        1 2023-01-03 12:00:14.000000 clr_loader-0.2.6/clr_loader.egg-info/not-zip-safe
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)       11 2023-08-07 15:22:56.000000 clr_loader-0.2.6/clr_loader.egg-info/requires.txt
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)       11 2023-08-07 15:22:56.000000 clr_loader-0.2.6/clr_loader.egg-info/top_level.txt
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:57.003004 clr_loader-0.2.6/doc/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)        8 2022-09-16 19:02:54.000000 clr_loader-0.2.6/doc/.gitignore
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      634 2022-09-16 19:02:54.000000 clr_loader-0.2.6/doc/Makefile
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      643 2022-10-15 07:15:18.000000 clr_loader-0.2.6/doc/conf.py
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      953 2022-09-16 19:02:54.000000 clr_loader-0.2.6/doc/index.rst
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      800 2022-09-16 19:02:54.000000 clr_loader-0.2.6/doc/make.bat
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      502 2022-09-16 19:02:54.000000 clr_loader-0.2.6/doc/reference.rst
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)       69 2022-09-23 05:27:39.000000 clr_loader-0.2.6/doc/requirements.txt
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     3350 2022-09-17 07:04:41.000000 clr_loader-0.2.6/doc/usage.rst
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:57.003004 clr_loader-0.2.6/example/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      631 2019-10-31 07:39:07.000000 clr_loader-0.2.6/example/TestClass.cs
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      526 2022-07-07 23:21:50.000000 clr_loader-0.2.6/example/example.csproj
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1720 2019-10-23 09:00:44.000000 clr_loader-0.2.6/example/example.sln
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:57.006337 clr_loader-0.2.6/netfx_loader/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     3545 2023-08-07 15:21:26.000000 clr_loader-0.2.6/netfx_loader/ClrLoader.cs
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)      838 2020-12-12 21:49:19.000000 clr_loader-0.2.6/netfx_loader/ClrLoader.csproj
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1777 2019-11-07 06:35:11.000000 clr_loader-0.2.6/netfx_loader/ClrLoader.sln
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1628 2021-02-13 17:01:41.000000 clr_loader-0.2.6/netfx_loader/DomainData.cs
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     1203 2022-10-15 07:15:28.000000 clr_loader-0.2.6/pyproject.toml
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)       38 2023-08-07 15:22:57.006337 clr_loader-0.2.6/setup.cfg
+-rwxr-xr-x   0 benedikt  (1000) benedikt  (1000)     4071 2022-10-15 07:15:18.000000 clr_loader-0.2.6/setup.py
+drwxr-xr-x   0 benedikt  (1000) benedikt  (1000)        0 2023-08-07 15:22:57.006337 clr_loader-0.2.6/tests/
+-rw-r--r--   0 benedikt  (1000) benedikt  (1000)     3960 2023-08-07 15:21:26.000000 clr_loader-0.2.6/tests/test_common.py
```

### Comparing `clr_loader-0.2.5/.github/workflows/ci-arm.yml` & `clr_loader-0.2.6/.github/workflows/ci-arm.yml`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/.github/workflows/ci.yml` & `clr_loader-0.2.6/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
   test:
     runs-on: ${{ matrix.os }}
     needs: build
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python: ['3.10', '3.9', '3.8', '3.7'] # pypy3
+        python: ['3.11', '3.10', '3.9', '3.8'] # pypy3
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Setup .NET
       uses: actions/setup-dotnet@v1
       with:
```

### Comparing `clr_loader-0.2.5/.github/workflows/docs.yml` & `clr_loader-0.2.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/.gitignore` & `clr_loader-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/LICENSE` & `clr_loader-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/PKG-INFO` & `clr_loader-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clr_loader
-Version: 0.2.5
+Version: 0.2.6
 Summary: Generic pure Python loader for .NET runtimes
 Author-email: Benedikt Reinartz <filmor@gmail.com>
 License: MIT
 Project-URL: Sources, https://github.com/pythonnet/clr-loader
 Project-URL: Documentation, https://pythonnet.github.io/clr-loader/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `clr_loader-0.2.5/README.md` & `clr_loader-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader/__init__.py` & `clr_loader-0.2.6/clr_loader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             - SIGUSR2
         This currently only works on POSIX platforms
     """
     from .mono import Mono
 
     libmono = _maybe_path(libmono)
     if libmono is None:
-        libmono = find_libmono(sgen=sgen)
+        libmono = find_libmono(sgen=sgen, assembly_dir=assembly_dir)
 
     impl = Mono(
         # domain=domain,
         debug=debug,
         jit_options=jit_options,
         config_file=_maybe_path(config_file),
         global_config_file=_maybe_path(global_config_file),
```

### Comparing `clr_loader-0.2.5/clr_loader/ffi/__init__.py` & `clr_loader-0.2.6/clr_loader/ffi/__init__.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader/ffi/hostfxr.py` & `clr_loader-0.2.6/clr_loader/ffi/hostfxr.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader/ffi/mono.py` & `clr_loader-0.2.6/clr_loader/ffi/mono.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader/hostfxr.py` & `clr_loader-0.2.6/clr_loader/hostfxr.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,31 +16,30 @@
         self._handle = None
 
         if _IS_SHUTDOWN:
             raise RuntimeError("Runtime can not be reinitialized")
 
         self._dotnet_root = Path(dotnet_root)
         self._dll = load_hostfxr(self._dotnet_root)
-        self._is_initialized = False
         self._handle = _get_handle(self._dll, self._dotnet_root, runtime_config)
-        self._load_func = _get_load_func(self._dll, self._handle)
+        self._load_func = None
 
         for key, value in params.items():
             self[key] = value
 
         # TODO: Get version
         self._version = "<undefined>"
 
     @property
     def dotnet_root(self) -> Path:
         return self._dotnet_root
 
     @property
     def is_initialized(self) -> bool:
-        return self._is_initialized
+        return self._load_func is not None
 
     @property
     def is_shutdown(self) -> bool:
         return _IS_SHUTDOWN
 
     def __getitem__(self, key: str) -> str:
         if self.is_shutdown:
@@ -77,42 +76,41 @@
             self._handle, size_ptr, keys_ptr, values_ptr
         )
         check_result(res)
 
         for i in range(size_ptr[0]):
             yield (decode(keys_ptr[i]), decode(values_ptr[i]))
 
+    def _get_load_func(self):
+        if self._load_func is None:
+            self._load_func = _get_load_func(self._dll, self._handle)
+
+        return self._load_func
+
     def _get_callable(self, assembly_path: StrOrPath, typename: str, function: str):
         # TODO: Maybe use coreclr_get_delegate as well, supported with newer API
         # versions of hostfxr
-        self._is_initialized = True
 
         # Append assembly name to typename
         assembly_path = Path(assembly_path)
         assembly_name = assembly_path.stem
         typename = f"{typename}, {assembly_name}"
 
         delegate_ptr = ffi.new("void**")
-        res = self._load_func(
+        res = self._get_load_func()(
             encode(str(assembly_path)),
             encode(typename),
             encode(function),
             ffi.NULL,
             ffi.NULL,
             delegate_ptr,
         )
         check_result(res)
         return ffi.cast("component_entry_point_fn", delegate_ptr[0])
 
-    def _check_initialized(self) -> None:
-        if self._handle is None:
-            raise RuntimeError("Runtime is shut down")
-        elif not self._is_initialized:
-            raise RuntimeError("Runtime is not initialized")
-
     def shutdown(self) -> None:
         if self._handle is not None:
             self._dll.hostfxr_close(self._handle)
             self._handle = None
 
     def info(self):
         return RuntimeInfo(
```

### Comparing `clr_loader-0.2.5/clr_loader/mono.py` & `clr_loader-0.2.6/clr_loader/mono.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     set_signal_chaining: bool = False,
 ) -> str:
     global _MONO, _ROOT_DOMAIN
     if _MONO is None:
         _MONO = load_mono(libmono)
 
         if assembly_dir is not None and config_dir is not None:
-            _MONO.mono_set_dirs(assembly_dir, config_dir)
+            _MONO.mono_set_dirs(assembly_dir.encode("utf8"), config_dir.encode("utf8"))
 
         # Load in global config (i.e /etc/mono/config)
         global_encoded = global_config_file or ffi.NULL
         _MONO.mono_config_parse(global_encoded)
 
         # Even if we don't have a domain config file, we still need to set it
         # as something, see https://github.com/pythonnet/clr-loader/issues/8
```

### Comparing `clr_loader-0.2.5/clr_loader/netfx.py` & `clr_loader-0.2.6/clr_loader/netfx.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 class NetFx(Runtime):
     def __init__(
         self, domain: Optional[str] = None, config_file: Optional[Path] = None
     ):
         initialize()
         if config_file is not None:
-            config_file_s = str(config_file)
+            config_file_s = str(config_file).encode("utf8")
         else:
             config_file_s = ffi.NULL
 
+        domain_s = domain.encode("utf8") if domain else ffi.NULL
+
         self._domain_name = domain
         self._config_file = config_file
-        self._domain = _FW.pyclr_create_appdomain(domain or ffi.NULL, config_file_s)
+        self._domain = _FW.pyclr_create_appdomain(domain_s, config_file_s)
 
     def info(self) -> RuntimeInfo:
         return RuntimeInfo(
             kind=".NET Framework",
             version="<undefined>",
             initialized=True,
             shutdown=_FW is None,
@@ -37,14 +39,19 @@
         func = _FW.pyclr_get_function(
             self._domain,
             str(Path(assembly_path)).encode("utf8"),
             typename.encode("utf8"),
             function.encode("utf8"),
         )
 
+        if func == ffi.NULL:
+            raise RuntimeError(
+                f"Failed to resolve {typename}.{function} from {assembly_path}"
+            )
+
         return func
 
     def shutdown(self):
         if self._domain and _FW:
             _FW.pyclr_close_appdomain(self._domain)
```

### Comparing `clr_loader-0.2.5/clr_loader/types.py` & `clr_loader-0.2.6/clr_loader/types.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader/util/__init__.py` & `clr_loader-0.2.6/clr_loader/util/__init__.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader/util/clr_error.py` & `clr_loader-0.2.6/clr_loader/util/clr_error.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader/util/coreclr_errors.py` & `clr_loader-0.2.6/clr_loader/util/coreclr_errors.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader/util/find.py` & `clr_loader-0.2.6/clr_loader/util/find.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     if dotnet_cli is not None:
         return find_runtimes_using_cli(dotnet_cli)
     else:
         dotnet_root = find_dotnet_root()
         return find_runtimes_in_root(dotnet_root)
 
 
-def find_libmono(*, sgen: bool = True) -> Path:
+def find_libmono(*, assembly_dir: str = None, sgen: bool = True) -> Path:
     """Find a suitable libmono dynamic library
 
     On Windows and macOS, we check the default installation directories.
 
     :param sgen:
         Whether to look for an SGen or Boehm GC instance. This parameter is
         ignored on Windows, as only ``sgen`` is installed with the default
@@ -133,15 +133,18 @@
     elif sys.platform == "darwin":
         path = (
             Path("/Library/Frameworks/Mono.framework/Versions/Current/lib")
             / f"lib{unix_name}.dylib"
         )
 
     else:
-        from ctypes.util import find_library
-
-        path = find_library(unix_name)
+        if assembly_dir == None:
+            from ctypes.util import find_library
+            path = find_library(unix_name)
+        else:
+            libname = "lib" + unix_name + ".so"
+            path = Path(assembly_dir) / "lib" / libname
 
     if path is None:
         raise RuntimeError("Could not find libmono")
 
     return Path(path)
```

### Comparing `clr_loader-0.2.5/clr_loader/util/hostfxr_errors.py` & `clr_loader-0.2.6/clr_loader/util/hostfxr_errors.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader/util/runtime_spec.py` & `clr_loader-0.2.6/clr_loader/util/runtime_spec.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/clr_loader.egg-info/PKG-INFO` & `clr_loader-0.2.6/clr_loader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clr-loader
-Version: 0.2.5
+Version: 0.2.6
 Summary: Generic pure Python loader for .NET runtimes
 Author-email: Benedikt Reinartz <filmor@gmail.com>
 License: MIT
 Project-URL: Sources, https://github.com/pythonnet/clr-loader
 Project-URL: Documentation, https://pythonnet.github.io/clr-loader/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `clr_loader-0.2.5/clr_loader.egg-info/SOURCES.txt` & `clr_loader-0.2.6/clr_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/doc/Makefile` & `clr_loader-0.2.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/doc/conf.py` & `clr_loader-0.2.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/doc/index.rst` & `clr_loader-0.2.6/doc/index.rst`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/doc/make.bat` & `clr_loader-0.2.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/doc/usage.rst` & `clr_loader-0.2.6/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/example/TestClass.cs` & `clr_loader-0.2.6/example/TestClass.cs`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/example/example.csproj` & `clr_loader-0.2.6/example/example.csproj`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/example/example.sln` & `clr_loader-0.2.6/example/example.sln`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/netfx_loader/ClrLoader.cs` & `clr_loader-0.2.6/netfx_loader/ClrLoader.cs`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,18 @@
         )
         {
             Print($"Creating AppDomain {name} with {configFile}");
             if (!string.IsNullOrEmpty(name))
             {
                 var setup = new AppDomainSetup
                 {
+                    ApplicationBase = AppDomain.CurrentDomain.BaseDirectory,
                     ConfigurationFile = configFile
                 };
+                Print($"Base: {AppDomain.CurrentDomain.BaseDirectory}");
                 var domain = AppDomain.CreateDomain(name, null, setup);
 
                 Print($"Located domain {domain}");
 
                 var domainData = new DomainData(domain);
                 _domains.Add(domainData);
                 return new IntPtr(_domains.Count - 1);
@@ -47,17 +49,17 @@
                 return IntPtr.Zero;
             }
         }
 
         [DllExport("pyclr_get_function", CallingConvention.Cdecl)]
         public static IntPtr GetFunction(
             IntPtr domain,
-            [MarshalAs(UnmanagedType.LPStr)] string assemblyPath,
-            [MarshalAs(UnmanagedType.LPStr)] string typeName,
-            [MarshalAs(UnmanagedType.LPStr)] string function
+            [MarshalAs(UnmanagedType.LPUTF8Str)] string assemblyPath,
+            [MarshalAs(UnmanagedType.LPUTF8Str)] string typeName,
+            [MarshalAs(UnmanagedType.LPUTF8Str)] string function
         )
         {
             try
             {
                 var domainData = _domains[(int)domain];
                 var deleg = domainData.GetEntryPoint(assemblyPath, typeName, function);
                 return Marshal.GetFunctionPointerForDelegate(deleg);
```

### Comparing `clr_loader-0.2.5/netfx_loader/ClrLoader.csproj` & `clr_loader-0.2.6/netfx_loader/ClrLoader.csproj`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/netfx_loader/ClrLoader.sln` & `clr_loader-0.2.6/netfx_loader/ClrLoader.sln`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/netfx_loader/DomainData.cs` & `clr_loader-0.2.6/netfx_loader/DomainData.cs`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/pyproject.toml` & `clr_loader-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clr_loader-0.2.5/setup.py` & `clr_loader-0.2.6/setup.py`

 * *Files identical despite different names*

