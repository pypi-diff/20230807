# Comparing `tmp/avro-to-python-etp-1.0.1.tar.gz` & `tmp/avro_to_python_etp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro-to-python-etp-1.0.1.tar", max compression
+gzip compressed data, was "avro_to_python_etp-1.0.2.tar", max compression
```

## Comparing `avro-to-python-etp-1.0.1.tar` & `avro_to_python_etp-1.0.2.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0     1074 2022-09-22 12:07:52.974411 avro-to-python-etp-1.0.1/LICENSE
--rw-r--r--   0        0        0     4785 2022-09-22 12:07:52.974411 avro-to-python-etp-1.0.1/README.rst
--rw-r--r--   0        0        0      163 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/__init__.py
--rw-r--r--   0        0        0     9800 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/avpr_to_avsc.py
--rw-r--r--   0        0        0        0 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/classes/__init__.py
--rw-r--r--   0        0        0     3047 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/classes/field.py
--rw-r--r--   0        0        0     1625 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/classes/file.py
--rw-r--r--   0        0        0      646 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/classes/node.py
--rw-r--r--   0        0        0      365 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/classes/reference.py
--rw-r--r--   0        0        0     1441 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/cli.py
--rw-r--r--   0        0        0       53 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/reader/__init__.py
--rw-r--r--   0        0        0     8339 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/reader/read.py
--rw-r--r--   0        0        0      449 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/baseTemplate.j2
--rw-r--r--   0        0        0     1615 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/arrayField.j2
--rw-r--r--   0        0        0      626 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/fieldFactory.j2
--rw-r--r--   0        0        0      644 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/mapField.j2
--rw-r--r--   0        0        0      536 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/primitiveField.j2
--rw-r--r--   0        0        0      125 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/referenceField.j2
--rw-r--r--   0        0        0      612 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/unionField.j2
--rw-r--r--   0        0        0      346 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/enum.j2
--rw-r--r--   0        0        0     1301 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/fixed.j2
--rw-r--r--   0        0        0      375 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/helpers.j2
--rw-r--r--   0        0        0      231 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/init.j2
--rw-r--r--   0        0        0       28 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/manifest.j2
--rw-r--r--   0        0        0     1856 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/pip_init.j2
--rw-r--r--   0        0        0        0 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/py.j2
--rw-r--r--   0        0        0      223 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/pyproject.j2
--rw-r--r--   0        0        0     2510 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/record.j2
--rw-r--r--   0        0        0      317 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/setup.j2
--rw-r--r--   0        0        0      348 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/imports/basicImports.j2
--rw-r--r--   0        0        0      221 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/imports/fileImports.j2
--rw-r--r--   0        0        0      285 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/partials/avroSchema.j2
--rw-r--r--   0        0        0       36 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/partials/footer.j2
--rw-r--r--   0        0        0      125 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/partials/header.j2
--rw-r--r--   0        0        0      159 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/partials/meta.j2
--rw-r--r--   0        0        0      238 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/templates/partials/objectSetter.j2
--rw-r--r--   0        0        0        0 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/__init__.py
--rw-r--r--   0        0        0        0 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/files/__init__.py
--rw-r--r--   0        0        0      445 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/files/enum.py
--rw-r--r--   0        0        0      441 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/files/fixed.py
--rw-r--r--   0        0        0      682 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/files/meta.py
--rw-r--r--   0        0        0     3056 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/files/record.py
--rw-r--r--   0        0        0     5385 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/helpers.py
--rw-r--r--   0        0        0      368 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/primitive_types.py
--rw-r--r--   0        0        0        0 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/__init__.py
--rw-r--r--   0        0        0     4052 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/array.py
--rw-r--r--   0        0        0     1404 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/enum.py
--rw-r--r--   0        0        0     4578 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/map.py
--rw-r--r--   0        0        0     1487 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/primitive.py
--rw-r--r--   0        0        0     1393 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/record.py
--rw-r--r--   0        0        0     1322 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/reference.py
--rw-r--r--   0        0        0     2222 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/type_factory.py
--rw-r--r--   0        0        0     3754 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/union.py
--rw-r--r--   0        0        0      330 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/exceptions.py
--rw-r--r--   0        0        0     3030 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/utils/paths.py
--rw-r--r--   0        0        0       56 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/writer/__init__.py
--rw-r--r--   0        0        0     9781 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/avro_to_python_etp/writer/writer.py
--rw-r--r--   0        0        0     1263 2022-09-22 12:07:52.978411 avro-to-python-etp-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6574 1970-01-01 00:00:00.000000 avro-to-python-etp-1.0.1/setup.py
--rw-r--r--   0        0        0     5900 1970-01-01 00:00:00.000000 avro-to-python-etp-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4785 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/README.rst
+-rw-r--r--   0        0        0      163 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/__init__.py
+-rw-r--r--   0        0        0     9800 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/avpr_to_avsc.py
+-rw-r--r--   0        0        0        0 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/classes/__init__.py
+-rw-r--r--   0        0        0     3047 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/classes/field.py
+-rw-r--r--   0        0        0     1625 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/classes/file.py
+-rw-r--r--   0        0        0      646 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/classes/node.py
+-rw-r--r--   0        0        0      365 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/classes/reference.py
+-rw-r--r--   0        0        0     1441 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/cli.py
+-rw-r--r--   0        0        0       53 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/reader/__init__.py
+-rw-r--r--   0        0        0     8339 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/reader/read.py
+-rw-r--r--   0        0        0      449 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/baseTemplate.j2
+-rw-r--r--   0        0        0     1615 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/arrayField.j2
+-rw-r--r--   0        0        0      626 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/fieldFactory.j2
+-rw-r--r--   0        0        0      644 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/mapField.j2
+-rw-r--r--   0        0        0      536 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/primitiveField.j2
+-rw-r--r--   0        0        0      125 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/referenceField.j2
+-rw-r--r--   0        0        0      612 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/unionField.j2
+-rw-r--r--   0        0        0      346 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/enum.j2
+-rw-r--r--   0        0        0     1301 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/fixed.j2
+-rw-r--r--   0        0        0      375 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/helpers.j2
+-rw-r--r--   0        0        0      231 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/init.j2
+-rw-r--r--   0        0        0       28 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/manifest.j2
+-rw-r--r--   0        0        0     1856 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/pip_init.j2
+-rw-r--r--   0        0        0        0 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/py.j2
+-rw-r--r--   0        0        0      223 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/pyproject.j2
+-rw-r--r--   0        0        0     2510 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/record.j2
+-rw-r--r--   0        0        0      317 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/setup.j2
+-rw-r--r--   0        0        0      348 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/imports/basicImports.j2
+-rw-r--r--   0        0        0      221 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/imports/fileImports.j2
+-rw-r--r--   0        0        0      285 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/partials/avroSchema.j2
+-rw-r--r--   0        0        0       36 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/partials/footer.j2
+-rw-r--r--   0        0        0      125 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/partials/header.j2
+-rw-r--r--   0        0        0      159 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/partials/meta.j2
+-rw-r--r--   0        0        0      238 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/templates/partials/objectSetter.j2
+-rw-r--r--   0        0        0        0 2023-08-07 13:56:05.657346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/files/__init__.py
+-rw-r--r--   0        0        0      445 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/files/enum.py
+-rw-r--r--   0        0        0      441 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/files/fixed.py
+-rw-r--r--   0        0        0      682 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/files/meta.py
+-rw-r--r--   0        0        0     3056 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/files/record.py
+-rw-r--r--   0        0        0     5385 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/helpers.py
+-rw-r--r--   0        0        0      368 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/primitive_types.py
+-rw-r--r--   0        0        0        0 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/__init__.py
+-rw-r--r--   0        0        0     4052 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/array.py
+-rw-r--r--   0        0        0     1404 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/enum.py
+-rw-r--r--   0        0        0     4578 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/map.py
+-rw-r--r--   0        0        0     1487 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/primitive.py
+-rw-r--r--   0        0        0     1393 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/record.py
+-rw-r--r--   0        0        0     1322 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/reference.py
+-rw-r--r--   0        0        0     2222 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/type_factory.py
+-rw-r--r--   0        0        0     3754 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/union.py
+-rw-r--r--   0        0        0      330 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/exceptions.py
+-rw-r--r--   0        0        0     3030 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/utils/paths.py
+-rw-r--r--   0        0        0       56 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/writer/__init__.py
+-rw-r--r--   0        0        0     9781 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/avro_to_python_etp/writer/writer.py
+-rw-r--r--   0        0        0     1257 2023-08-07 13:56:05.661346 avro_to_python_etp-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5902 1970-01-01 00:00:00.000000 avro_to_python_etp-1.0.2/PKG-INFO
```

### Comparing `avro-to-python-etp-1.0.1/LICENSE` & `avro_to_python_etp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/README.rst` & `avro_to_python_etp-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/avpr_to_avsc.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/avpr_to_avsc.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/classes/field.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/classes/field.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/classes/file.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/classes/file.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/classes/node.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/classes/node.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/cli.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/cli.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/reader/read.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/reader/read.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/arrayField.j2` & `avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/arrayField.j2`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/fieldFactory.j2` & `avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/fieldFactory.j2`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/mapField.j2` & `avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/mapField.j2`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/primitiveField.j2` & `avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/primitiveField.j2`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/templates/fields/unionField.j2` & `avro_to_python_etp-1.0.2/avro_to_python_etp/templates/fields/unionField.j2`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/fixed.j2` & `avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/fixed.j2`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/pip_init.j2` & `avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/pip_init.j2`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/templates/files/record.j2` & `avro_to_python_etp-1.0.2/avro_to_python_etp/templates/files/record.j2`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/files/meta.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/files/meta.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/files/record.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/files/record.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/helpers.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/helpers.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/array.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/array.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/enum.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/enum.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/map.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/map.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/primitive.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/primitive.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/record.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/record.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/reference.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/reference.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/type_factory.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/type_factory.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/avro/types/union.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/avro/types/union.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/utils/paths.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/utils/paths.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/avro_to_python_etp/writer/writer.py` & `avro_to_python_etp-1.0.2/avro_to_python_etp/writer/writer.py`

 * *Files identical despite different names*

### Comparing `avro-to-python-etp-1.0.1/pyproject.toml` & `avro_to_python_etp-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avro-to-python-etp"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   "Scott Rothbarth <srserves85@gmail.com>",
   "Lionel Untereiner <lionel.untereiner@geosiris.com>",
   "Valentin Gauthier <valentin.gauthier@geosiris.com>"
 ]
 description = "Light tool for compiling avro schema files (.avsc) to python classes making using avro schemata easy."
 readme = "README.rst"
@@ -22,15 +22,15 @@
 "Bug Tracker" = "https://github.com/geosiris-technologies/avro-to-python-etp/issues"
 
 [build-system]
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.11"
+python = "^3.8"
 Jinja2 = "^3.1.2"
 click = "^8.1.3"
 anytree = "^2.8.0"
 nested-lookup = "^0.2.25"
 typingx = "^0.6.0"
 wheel = "^0.37.1"
 avro = "^1.11.1"
```

### Comparing `avro-to-python-etp-1.0.1/PKG-INFO` & `avro_to_python_etp-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: avro-to-python-etp
-Version: 1.0.1
+Version: 1.0.2
 Summary: Light tool for compiling avro schema files (.avsc) to python classes making using avro schemata easy.
 Home-page: https://github.com/geosiris-technologies/avro-to-python-etp
 License: MIT
 Keywords: avro,etp
 Author: Scott Rothbarth
 Author-email: srserves85@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: anytree (>=2.8.0,<3.0.0)
 Requires-Dist: avro (>=1.11.1,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: nested-lookup (>=0.2.25,<0.3.0)
 Requires-Dist: typingx (>=0.6.0,<0.7.0)
 Requires-Dist: wheel (>=0.37.1,<0.38.0)
```

