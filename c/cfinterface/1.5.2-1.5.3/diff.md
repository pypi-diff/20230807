# Comparing `tmp/cfinterface-1.5.2.tar.gz` & `tmp/cfinterface-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfinterface-1.5.2.tar", last modified: Tue Aug  1 00:53:18 2023, max compression
+gzip compressed data, was "cfinterface-1.5.3.tar", last modified: Mon Aug  7 14:17:21 2023, max compression
```

## Comparing `cfinterface-1.5.2.tar` & `cfinterface-1.5.3.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.364179 cfinterface-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 00:52:01.000000 cfinterface-1.5.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-01 00:53:18.364179 cfinterface-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-01 00:52:01.000000 cfinterface-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.352179 cfinterface-1.5.2/cfinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.352179 cfinterface-1.5.2/cfinterface/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.352179 cfinterface-1.5.2/cfinterface/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.352179 cfinterface-1.5.2/cfinterface/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/adapters/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.352179 cfinterface-1.5.2/cfinterface/adapters/components/line/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/adapters/components/line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/adapters/components/line/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/adapters/components/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.356179 cfinterface-1.5.2/cfinterface/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/adapters/reading/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.356179 cfinterface-1.5.2/cfinterface/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/adapters/writing/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.356179 cfinterface-1.5.2/cfinterface/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/components/section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.356179 cfinterface-1.5.2/cfinterface/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/data/blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/data/registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/data/sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.356179 cfinterface-1.5.2/cfinterface/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/files/blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/files/registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/files/sectionfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.356179 cfinterface-1.5.2/cfinterface/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/reading/blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/reading/registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/reading/sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.360179 cfinterface-1.5.2/cfinterface/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/writing/blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/writing/registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-01 00:52:01.000000 cfinterface-1.5.2/cfinterface/writing/sectionwriting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.352179 cfinterface-1.5.2/cfinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-01 00:53:18.000000 cfinterface-1.5.2/cfinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-01 00:53:18.000000 cfinterface-1.5.2/cfinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:53:18.000000 cfinterface-1.5.2/cfinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 00:53:18.000000 cfinterface-1.5.2/cfinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 00:53:18.000000 cfinterface-1.5.2/cfinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.360179 cfinterface-1.5.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:53:18.364179 cfinterface-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-01 00:52:01.000000 cfinterface-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.360179 cfinterface-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.360179 cfinterface-1.5.2/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.360179 cfinterface-1.5.2/tests/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/components/test_blockrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/components/test_linerepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/components/test_registerrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/components/test_sectionrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.360179 cfinterface-1.5.2/tests/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/reading/test_readingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.360179 cfinterface-1.5.2/tests/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/adapters/writing/test_writingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.360179 cfinterface-1.5.2/tests/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/components/test_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.360179 cfinterface-1.5.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/data/test_blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/data/test_registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/data/test_sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.364179 cfinterface-1.5.2/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/files/test_blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/files/test_registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/files/test_sectionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.364179 cfinterface-1.5.2/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.364179 cfinterface-1.5.2/tests/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/reading/test_blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/reading/test_registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/reading/test_sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:53:18.364179 cfinterface-1.5.2/tests/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/writing/test_blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/writing/test_registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-01 00:52:01.000000 cfinterface-1.5.2/tests/writing/test_sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 14:16:06.000000 cfinterface-1.5.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-07 14:17:21.401047 cfinterface-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-07 14:16:06.000000 cfinterface-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/components/line/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/components/line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/components/line/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/components/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/reading/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/adapters/writing/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/components/section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/data/blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/data/registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/data/sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/cfinterface/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/files/blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/files/registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/files/sectionfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/cfinterface/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/reading/blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/reading/registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/reading/sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/cfinterface/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/writing/blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/writing/registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-07 14:16:06.000000 cfinterface-1.5.3/cfinterface/writing/sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.393047 cfinterface-1.5.3/cfinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 14:17:21.000000 cfinterface-1.5.3/cfinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:17:21.401047 cfinterface-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-07 14:16:06.000000 cfinterface-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/test_blockrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/test_linerepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/test_registerrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/components/test_sectionrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/reading/test_readingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/adapters/writing/test_writingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.397047 cfinterface-1.5.3/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/components/test_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/data/test_blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/data/test_registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/data/test_sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/files/test_blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/files/test_registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/files/test_sectionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/reading/test_blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/reading/test_registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/reading/test_sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:17:21.401047 cfinterface-1.5.3/tests/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/writing/test_blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/writing/test_registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-07 14:16:06.000000 cfinterface-1.5.3/tests/writing/test_sectionwriting.py
```

### Comparing `cfinterface-1.5.2/LICENSE.md` & `cfinterface-1.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/PKG-INFO` & `cfinterface-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.5.2
+Version: 1.5.3
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.5.2/README.md` & `cfinterface-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/adapters/components/line/repository.py` & `cfinterface-1.5.3/cfinterface/adapters/components/line/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/adapters/components/repository.py` & `cfinterface-1.5.3/cfinterface/adapters/components/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/adapters/reading/repository.py` & `cfinterface-1.5.3/cfinterface/adapters/reading/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/adapters/writing/repository.py` & `cfinterface-1.5.3/cfinterface/adapters/writing/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/block.py` & `cfinterface-1.5.3/cfinterface/components/block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/datetimefield.py` & `cfinterface-1.5.3/cfinterface/components/datetimefield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/defaultblock.py` & `cfinterface-1.5.3/cfinterface/components/defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/defaultregister.py` & `cfinterface-1.5.3/cfinterface/components/defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/defaultsection.py` & `cfinterface-1.5.3/cfinterface/components/defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/field.py` & `cfinterface-1.5.3/cfinterface/components/field.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/floatfield.py` & `cfinterface-1.5.3/cfinterface/components/floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/integerfield.py` & `cfinterface-1.5.3/cfinterface/components/integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/line.py` & `cfinterface-1.5.3/cfinterface/components/line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/literalfield.py` & `cfinterface-1.5.3/cfinterface/components/literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/register.py` & `cfinterface-1.5.3/cfinterface/components/register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/components/section.py` & `cfinterface-1.5.3/cfinterface/components/section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/data/blockdata.py` & `cfinterface-1.5.3/cfinterface/data/blockdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,14 +144,30 @@
         if len(filtered_blocks) == 0:
             return None
         elif len(filtered_blocks) == 1:
             return filtered_blocks[0]
         else:
             return filtered_blocks
 
+    def remove_blocks_of_type(self, t: Type[T], **kwargs):
+        """
+        Removes a set of blocks given a type and an optional group of
+        filters, similar to `get_blocks_of_type()`
+
+        :param t: The block type that is desired
+        :type t: Type[T]
+        """
+        filtered_blocks = self.get_blocks_of_type(t, **kwargs)
+        if isinstance(filtered_blocks, Block):
+            self.remove(filtered_blocks)
+        elif isinstance(filtered_blocks, list):
+            for b in filtered_blocks:
+                if isinstance(b, Block) and b != self.__root:
+                    self.remove(b)
+
     @property
     def first(self) -> Block:
         return self.__root
 
     @property
     def last(self) -> Block:
         return self.__head
```

### Comparing `cfinterface-1.5.2/cfinterface/data/registerdata.py` & `cfinterface-1.5.3/cfinterface/data/registerdata.py`

 * *Files 14% similar despite different names*

```diff
@@ -143,14 +143,32 @@
         if len(filtered_registers) == 0:
             return None
         elif len(filtered_registers) == 1:
             return filtered_registers[0]
         else:
             return filtered_registers
 
+    def remove_registers_of_type(self, t: Type[T], **kwargs):
+        """
+        Removes a set of registers given a type and an optional group of
+        filters, similar to `get_registers_of_type()`
+
+        :param t: The register type that is desired
+        :type t: Type[T]
+        """
+        filtered_registers = self.get_registers_of_type(t, **kwargs)
+        if isinstance(filtered_registers, t) and isinstance(
+            filtered_registers, Register
+        ):
+            self.remove(filtered_registers)
+        elif isinstance(filtered_registers, list):
+            for r in filtered_registers:
+                if isinstance(r, Register) and r != self.__root:
+                    self.remove(r)
+
     @property
     def first(self) -> Register:
         return self.__root
 
     @property
     def last(self) -> Register:
         return self.__head
```

### Comparing `cfinterface-1.5.2/cfinterface/data/sectiondata.py` & `cfinterface-1.5.3/cfinterface/data/sectiondata.py`

 * *Files 26% similar despite different names*

```diff
@@ -144,14 +144,32 @@
         if len(filtered_sections) == 0:
             return None
         elif len(filtered_sections) == 1:
             return filtered_sections[0]
         else:
             return filtered_sections
 
+    def remove_sections_of_type(self, t: Type[T], **kwargs):
+        """
+        Removes a set of sections given a type and an optional group of
+        filters, similar to `get_sections_of_type()`
+
+        :param t: The section type that is desired
+        :type t: Type[T]
+        """
+        filtered_sections = self.get_sections_of_type(t, **kwargs)
+        if isinstance(filtered_sections, t) and isinstance(
+            filtered_sections, Section
+        ):
+            self.remove(filtered_sections)
+        elif isinstance(filtered_sections, list):
+            for s in filtered_sections:
+                if isinstance(s, Section) and s != self.__root:
+                    self.remove(s)
+
     @property
     def first(self) -> Section:
         return self.__root
 
     @property
     def last(self) -> Section:
         return self.__head
```

### Comparing `cfinterface-1.5.2/cfinterface/files/blockfile.py` & `cfinterface-1.5.3/cfinterface/files/blockfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/files/registerfile.py` & `cfinterface-1.5.3/cfinterface/files/registerfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/files/sectionfile.py` & `cfinterface-1.5.3/cfinterface/files/sectionfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/reading/blockreading.py` & `cfinterface-1.5.3/cfinterface/reading/blockreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/reading/registerreading.py` & `cfinterface-1.5.3/cfinterface/reading/registerreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/reading/sectionreading.py` & `cfinterface-1.5.3/cfinterface/reading/sectionreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/writing/blockwriting.py` & `cfinterface-1.5.3/cfinterface/writing/blockwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/writing/registerwriting.py` & `cfinterface-1.5.3/cfinterface/writing/registerwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface/writing/sectionwriting.py` & `cfinterface-1.5.3/cfinterface/writing/sectionwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/cfinterface.egg-info/PKG-INFO` & `cfinterface-1.5.3/cfinterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.5.2
+Version: 1.5.3
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.5.2/cfinterface.egg-info/SOURCES.txt` & `cfinterface-1.5.3/cfinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/setup.py` & `cfinterface-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/adapters/components/test_linerepository.py` & `cfinterface-1.5.3/tests/adapters/components/test_linerepository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_block.py` & `cfinterface-1.5.3/tests/components/test_block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_datetimefield.py` & `cfinterface-1.5.3/tests/components/test_datetimefield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_defaultblock.py` & `cfinterface-1.5.3/tests/components/test_defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_defaultregister.py` & `cfinterface-1.5.3/tests/components/test_defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_defaultsection.py` & `cfinterface-1.5.3/tests/components/test_defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_floatfield.py` & `cfinterface-1.5.3/tests/components/test_floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_integerfield.py` & `cfinterface-1.5.3/tests/components/test_integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_line.py` & `cfinterface-1.5.3/tests/components/test_line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_literalfield.py` & `cfinterface-1.5.3/tests/components/test_literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_register.py` & `cfinterface-1.5.3/tests/components/test_register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/components/test_section.py` & `cfinterface-1.5.3/tests/components/test_section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/data/test_blockdata.py` & `cfinterface-1.5.3/tests/data/test_blockdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,7 +121,16 @@
 def test_blockdata_get_blocks_of_type_filter():
     b1 = DummyBlock(data=10)
     bd = BlockData(b1)
     bd.append(DummyBlock())
     bd.append(DummyBlock(data=11))
     assert len(bd.get_blocks_of_type(DummyBlock)) == 3
     assert bd.get_blocks_of_type(DummyBlock, my_data=10) == b1
+
+
+def test_blockdata_remove_blocks_of_type_no_filter():
+    b1 = DummyBlock(data=10)
+    bd = BlockData(b1)
+    bd.append(DummyBlock())
+    bd.append(DummyBlock(data=11))
+    bd.remove_blocks_of_type(DummyBlock)
+    assert len(bd) == 1
```

### Comparing `cfinterface-1.5.2/tests/data/test_registerdata.py` & `cfinterface-1.5.3/tests/data/test_registerdata.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,21 +104,30 @@
 def test_registerdata_of_type():
     rd = RegisterData(DummyRegister())
     rd.append(DummyRegister())
     assert len(rd) == 2
     assert len([b for b in rd.of_type(DummyRegister)]) == 2
 
 
-def test_RegisterData_get_registers_of_type_no_filter():
+def test_registerdata_get_registers_of_type_no_filter():
     r1 = DummyRegister(data=[10])
     rd = RegisterData(r1)
     rd.append(Register())
     assert rd.get_registers_of_type(DummyRegister) == r1
 
 
-def test_RegisterData_get_registers_of_type_filter():
+def test_registerdata_get_registers_of_type_filter():
     r1 = DummyRegister(data=[10])
     rd = RegisterData(r1)
     rd.append(DummyRegister())
     rd.append(DummyRegister(data=[11]))
     assert len(rd.get_registers_of_type(DummyRegister)) == 3
     assert rd.get_registers_of_type(DummyRegister, my_data=10) == r1
+
+
+def test_registerdata_remove_registers_of_type_no_filter():
+    r1 = DummyRegister(data=[10])
+    rd = RegisterData(r1)
+    rd.append(DummyRegister())
+    rd.append(DummyRegister(data=[11]))
+    rd.remove_registers_of_type(DummyRegister)
+    assert len(rd) == 1
```

### Comparing `cfinterface-1.5.2/tests/data/test_sectiondata.py` & `cfinterface-1.5.3/tests/data/test_sectiondata.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,7 +118,16 @@
 def test_sectiondata_get_sections_of_type_filter():
     b1 = DummySection(data=10)
     bd = SectionData(b1)
     bd.append(DummySection())
     bd.append(DummySection(data=11))
     assert len(bd.get_sections_of_type(DummySection)) == 3
     assert bd.get_sections_of_type(DummySection, my_data=10) == b1
+
+
+def test_sectiondata_remove_sections_of_type_no_filter():
+    b1 = DummySection(data=10)
+    bd = SectionData(b1)
+    bd.append(DummySection())
+    bd.append(DummySection(data=11))
+    bd.remove_sections_of_type(DummySection)
+    assert len(bd) == 1
```

### Comparing `cfinterface-1.5.2/tests/files/test_blockfile.py` & `cfinterface-1.5.3/tests/files/test_blockfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/files/test_registerfile.py` & `cfinterface-1.5.3/tests/files/test_registerfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/files/test_sectionfile.py` & `cfinterface-1.5.3/tests/files/test_sectionfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/mocks/mock_open.py` & `cfinterface-1.5.3/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/reading/test_blockreading.py` & `cfinterface-1.5.3/tests/reading/test_blockreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/reading/test_registerreading.py` & `cfinterface-1.5.3/tests/reading/test_registerreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/reading/test_sectionreading.py` & `cfinterface-1.5.3/tests/reading/test_sectionreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/writing/test_blockwriting.py` & `cfinterface-1.5.3/tests/writing/test_blockwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/writing/test_registerwriting.py` & `cfinterface-1.5.3/tests/writing/test_registerwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.5.2/tests/writing/test_sectionwriting.py` & `cfinterface-1.5.3/tests/writing/test_sectionwriting.py`

 * *Files identical despite different names*

